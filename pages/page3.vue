<template>
  <div class="container col-10">

    <div class="row">
      
      <!-- pasos -->
        <div 
            class="col-md-3 mt-5" 
            style="color: #00a2c2;"
        >         
            <h4>
                Definición
                <span
                    class="badge badge-primary float-left step"
                >
                    {{ page }}
                </span>
            </h4>
        </div>

      <!-- agregar archivo -->
      <div class="col">
        <Archivo />
      </div>
    </div>
  </div>
</template>

<script>
import Archivo from '@/components/page3/Archivo'
export default {
  components: {
    Archivo
  },
  data(){
    return {
      page: '3/4'
    }
  }
}
</script>

<style>
.step {
    height: 40px;
    display: flex;
    border-radius: 50%;
    margin-right: 0.4em;
    align-items: center;
    background-color: #00a2c2;
}
</style>
