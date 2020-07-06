<template>
    <div class="container col-10">
      <div class="row">
        
        <!-- pasos -->
        <div 
            class="col-md-3 mt-5" 
            style="color: #00a2c2;"
        >         
            <h4>
                <span
                    class="badge badge-primary float-left step"
                >
                    {{ page }}
                </span>
                Especialidad
            </h4>
        </div>
        
        <!-- categorias -->
        <div class="col">
           <Listas />
        </div>

      </div>
    </div>      
</template>

<script>
import Listas from '@/components/page2/Listas'
export default {
    components: {
        Listas
    },
    data: () => ({
        page: '2/4'
    })
}
</script>

<style scoped>
.step {
    height: 40px;
    display: flex;
    border-radius: 50%;
    margin-right: 20px;
    align-items: center;
    background-color: #00a2c2;
}
</style>