<template>
    <div class="container col-10">
      <div class="row">
        
        <!-- pasos -->
        <div
            class="col-md-3 mt-5" 
            style="color: #00a2c2;"
        >         
            <h4>
                Tipo de Presentación
                <span
                    class="badge badge-primary float-left step"
                >
                    {{ page }}
                </span>
            </h4>
        </div>

        <div class="col">
            <Modos />
        </div>

      </div>
    </div>      
</template>

<script>
import Modos from '@/components/page4/Modos'
export default {
    components: {
        Modos
    },
    data: () => ({
        page: '4/4'
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