<template>
  <div class="container col-10">

    <div class="row">
      
      <!-- pasos -->
        <div class="col-md-3 mt-5" style="color: #00a2c2;" >         
            <h4> Definición
                <span class="badge badge-primary float-left step">
                    {{ page }}
                </span>
            </h4>
        </div>

      <div class="col">
        <Formulario />
      </div>

    </div>
  </div>
</template>

<script>
import Formulario from '@/components/page1/Formulario'
export default {
  components: {
    Formulario
  },
  data(){
    return {
      page: '1/4'
    }
  }
}
</script>

<style>
.step {
    height: 40px;
    display: flex;
    border-radius: 50%;
    margin-right: 20px;
    align-items: center;
    background-color: #00a2c2;
}
</style>
