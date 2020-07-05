<template>
<div>
  <!-- listas de opciones -->
  <div class="mt-5">
      <P>Marca dentro del área elegida, la categoría y subcategoría que correspondan*:</P>
  </div>  


  <div class="list-group list-group-flush">
    <!-- lista -->
    <button type="button" v-for="(boton, i) in botones" :key="i" class="hov list-group-item list-group-item-action btn btn-outline-light">
      {{ boton.titulo }}
    </button>    
  </div>

  <Add3 />

</div>
</template>

<script>
import Add3 from '@/components/page2/agregar/Add3'
export default {
  components: {
    Add3
  },
  data: () => ({
    botones: [
      {
        titulo:
          'Creatividad Publicitaria'
      },
      {
        titulo:
          'Planificación de Medios'
      },
      {
        titulo:
          'Publicidad Digital'
      },
      {
        titulo:
          'Gestión de Campaña Publicitaria'
      },
      {
        titulo:
          'Publicidad en Redes Sociales (Social Ads)'
      },
      {
        titulo:
          'Publicidad BTL'
      },
      {
        titulo:
          'Eventos'
      },
      {
        titulo:
          'Prensa'
      },
      {
        titulo:
          'Estrategia multiformato 360'
      }
    ]
  })
}
</script>

<style scoped>
.hov:focus {
  background-color: #0e76bc;
  color: white;
}
.hov:hover {
  background-color: #0e76bc;
  color: white;
}
</style>