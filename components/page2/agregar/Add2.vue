<template>
    <!-- slector  -->
    <div>
      <p class="mt-5">Si lo deseas, puedes agregar hasta 5 habilidades que consideres necesarias.</p>

      <div class="input-group mb-3 input-group-lg">
        <input type="text" class="form-control" v-model="nuevoBoton" @keyup.enter="agregarNombre" placeholder="AUTOCOMPLETE" aria-label="Recipient's username" aria-describedby="button-addon2">
        <div class="input-group-append">

          <button class="btn btn-secondary btn btn-ligh btn-lg" @click="agregarNombre" type="button" id="button-addon2">Agregar +</button>
        </div>
      </div>

      <div v-for="(boton, i) in botones" :key="i" class="btn-group">        
        <span class="badge badge-light btn rounded-circle delete" @click="eliminar(i)">X</span>        
        <div 
          class="btn mx-3 boton">{{ boton.nombre }}
        </div>      
      </div>

    </div>
</template>

<script>
export default {
  data(){
    return {
      botones: [],
      nuevoBoton: ''
  }  
 },
  methods: {
    agregarNombre () {
      this.botones.push({
        nombre: this.nuevoBoton
      })
      this.nuevoBoton = ''
    },
    eliminar(i) {
      this.botones.splice(i, 1)
      
    }
  }
}
</script>

<style scoped>
.delete {
  z-index: 2;
  margin-left: 6px;
  position: absolute;
  border: 0.6px solid;
}
.boton {
  height: 40px;
  border: none;
  color: white;
  background-color: #fcb040;
}
.boton::after {
    top: 1px;
    width: 0; 
    height: 0; 
    content: "";
    right: -18px;
    position: absolute;
    border-left: 19px solid #fcb040;
    border-top: 19px solid transparent;
    border-bottom: 19px solid transparent;
}

</style>