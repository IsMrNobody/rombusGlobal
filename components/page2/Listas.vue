<template>
    <div>
        <div class="mt-5 mb-5">
            <h2>Selecciona el area profesional adecuada</h2>
            <P>Elige el servicio que enfoca tu necesidad principal:</P>
        </div>

        <!-- cards -->
        <div class="card-group card-deck">
            <div class="card shadow justify-content-center">
                <button class="btn btn-outline-light carta1 tam" @click="activar" >
                    <div class="card-title">                    
                    <img src="/icons/binoculars.svg" path="red" height="30" class="my-2 colr">
                    <h5>Estrategia y marketin</h5>
                    </div>
                </button>
            </div>
            <div class="card shadow justify-content-center">
                <button class="btn btn-outline-light carta2 tam" @click="activar2">
                    <div class="card-title">
                    <img src="/icons/eye.svg" height="30" class="mr-auto my-2">
                    <h5>Diseño y Creatividad</h5>
                    </div>
                </button>
            </div>
            <div class="card shadow justify-content-center">
                <button class="btn btn-outline-light carta3 tam" @click="activar3">
                    <div class="card-title">
                    <img src="/icons/thumbs.svg" height="30" class="mr-auto my-2">
                    <h5>Publicidad y Campañas</h5>
                    </div>
                </button>
            </div>
            <div class="card shadow justify-content-center">
                <button class="btn btn-outline-light carta4 tam" @click="activar4">
                    <div class="card-title">
                    <img src="/icons/code.svg" height="30" class="mr-auto my-2">
                    <h5>Programción y Tecnología</h5>
                    </div>
                </button>
            </div>

        </div>

        <Lista1 v-if="mostrar" />
        <Lista2 v-if="mostrar2" />
        <Lista3 v-if="mostrar3" />
        <Lista4 v-if="mostrar4" />

        <!-- boton continuar -->
        <div class="d-flex justify-content-between mb-5">
            <nuxt-link to="/">
                <button type="button" class="my-5 btn btn-link" style="color: #00a2c2;">Atras</button>
            </nuxt-link>
            <nuxt-link to="/page3">
                <button type="button" class="button btn btn-outline-dark my-5 btn-lg" style="background-color: #00a2c2;">Continuar</button>
            </nuxt-link>
        </div>
    </div>
</template>

<script>
import Lista1 from '@/components/page2/listas/Lista1'
import Lista2 from '@/components/page2/listas/Lista2'
import Lista3 from '@/components/page2/listas/Lista3'
import Lista4 from '@/components/page2/listas/Lista4'
export default {
    components: {
        Lista1,
        Lista2,
        Lista3,
        Lista4
    },
    data: () => ({
        page: '2/4',
        mostrar: false,
        mostrar2: false,
        mostrar3: false,
        mostrar4: false
    }),
    methods: {
        activar() {
            this.mostrar = true
            this.mostrar2 = false
            this.mostrar3 = false
            this.mostrar4 = false
        },
        activar2() {
            this.mostrar2 = true
            this.mostrar3 = false
            this.mostrar4 = false
            this.mostrar = false
        },
        activar3() {
            this.mostrar3 = true
            this.mostrar4 = false
            this.mostrar2 = false
            this.mostrar = false
        },
        activar4() {
            this.mostrar4 = true
            this.mostrar3 = false
            this.mostrar2 = false
            this.mostrar = false
        },
    }
}
</script>

<style scoped>
.tam{    
    height: 200px;
}
.carta1, .carta2, .carta3, .carta4{
    color: black;
}
.carta1:focus{
    background: #d01d00;
    color: white;
}
.carta2:focus{
    background: #fcb040;
    color: white;
}
.carta3:focus{
    background: #0e76bc;
    color: white;
}
.carta4:focus{
    background: #9f1f63;
    color: white;
}
p {
    font-size: 18px;
}
.button {
  border: none;
  width: 300px;
  color: white;
  font-size: 24px;
  margin: 4px 2px;
  cursor: pointer;
  text-align: center;
  padding: 16px 32px;
  text-decoration: none;
}
</style>