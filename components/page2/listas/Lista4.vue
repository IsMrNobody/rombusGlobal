<template>
<div>
  <!-- listas de opciones -->
  <div class="mt-5">
      <P>Marca dentro del área elegida, la categoría y subcategoría que correspondan*:</P>
  </div>  


  <div class="list-group list-group-flush">
    <!-- lista -->
    <button 
      type="button" 
      v-for="(boton, i) in botones" :key="i" 
      class="hov list-group-item list-group-item-action btn btn-outline-light">
      {{ boton.titulo }}
    </button>    
  </div>

  <Add4 />

</div>
</template>

<script>
import Add4 from '@/components/page2/agregar/Add4'
export default {
  components: {
    Add4
  },
  data: () => ({
    botones: [
      {
        titulo:
          'Interfaz de Usuario - Diseño UI / Front-End'
      },
      {
        titulo:
          'Programación Web'
      },
      {
        titulo:
          'Plataforma de Gestión de Contenidos (CMS)'
      },
      {
        titulo:
          'Desarrollo de Aplicaciones'
      },
      {
        titulo:
          'Integración con API’s'
      },
      {
        titulo:
          'Comercio Electrónico'
      },
      {
        titulo:
          'Juegos'
      },
      {
        titulo:
          'Control de Calidad'
      },
      {
        titulo:
          'Sistemas'
      },
      {
        titulo:
          'Redes'
      },
      {
        titulo:
          'Seguridad Informática'
      },
      {
        titulo:
          'Estrategia de Ventas on line'
      },
      {
        titulo:
          'Inteligencia de Negocios / BI (Business Intelligence)'
      },
      {
        titulo:
          'Soporte'
      }
    ]
  })
}
</script>

<style scoped>
.hov:focus {
  color: white;
  background-color: #9f1f63;
}
.hov:hover {
  color: white;
  background-color: #9f1f63;
}
</style>