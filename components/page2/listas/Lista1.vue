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

  <!-- Agregar categoria -->
  <Add />

</div>
</template>

<script>
import Add from '@/components/page2/agregar/Add'
export default {
  components: {
    Add
  },
  data: () => ({
    botones: [
      {
        titulo:
          'Desarrollo de Negocio Digital'
      },
      {
        titulo:
          'Marca e Imagen Corporativa  / Branding'
      },
      {
        titulo:
          'Estrategia de Contenidos y Comunicación'
      },
      {
        titulo:
          'Marketing de Social Media'
      },
      {
        titulo:
          'Reputación on line'
      },
      {
        titulo:
          'Estrategia de Crecimiento (Growth Hacking)'
      },
      {
        titulo:
          'Estrategia de Experiencia de Consumidor'
      },
      {
        titulo:
          'Generación de Prospectos (Leads)'
      },
      {
        titulo:
          'Gestión de Campaña Digital'
      },
      {
        titulo:
          'Optimización en Buscadores (SEO)'
      },
      {
        titulo:
          'Marketing en Buscadores (SEM)'
      },
      {
        titulo:
          'Estrategia de Ventas on line'
      },
      {
        titulo:
          'Relaciones Públicas'
      },
      {
        titulo:
          'Marketing de Influencers'
      },
      {
        titulo:
          'Investigación y Análisis de Mercado'
      }
    ]
  })
}
</script>

<style scoped>
.hov:focus {
  background-color: #d01d00;
  color: white;
}
.hov:hover {
  background-color: #d01d00;
  color: white;
}
</style>