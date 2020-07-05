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

  <Add2 />

</div>
</template>

<script>
import Add2 from '@/components/page2/agregar/Add2'
export default {
  components: {
    Add2
  },
  data: () => ({
    botones: [
      {
        titulo:
          'Creación de Marca e Identidad Corporativa'
      },
      {
        titulo:
          'Diseño Web '
      },
      {
        titulo:
          'Diseño UX: Experiencia de Usuario'
      },
      {
        titulo:
          'Diseño Gráfico'
      },
      {
        titulo:
          'Diseño Editorial'
      },
      {
        titulo:
          'Diseño Industrial'
      },
      {
        titulo:
          'Diseño de Indumentaria y Moda'
      },
      {
        titulo:
          'Redacción'
      },
      {
        titulo:
          'Traducción a idiomas'
      },
      {
        titulo:
          'Fotografía'
      },
      {
        titulo:
          'Ilustraciones'
      },
      {
        titulo:
          'Animaciones'
      },
      {
        titulo:
          'Video'
      },
      {
        titulo:
          'Audio y Sonido'
      }
    ]
  })
}
</script>

<style scoped>
.hov:focus {
  background-color: #fcb040;
  color: white;
}
.hov:hover {
  background-color: #fcb040;
  color: white;
}
.linea {
  border: none;
}
</style>