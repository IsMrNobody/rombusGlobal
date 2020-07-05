<template>
    <div class="container col-10">
      <div class="row">        
            <!-- pasos -->
            <div class="col-md-3">
                <div 
                    v-for="(item, i) in pasos" :key="i"
                    class="mt-5 top" 
                    style="color: #00a2c2;"
                >
                    <h4>
                        {{ item.name }}
                        <span
                            class="badge badge-primary float-left step mx-4"
                        >
                            {{ item.page }}
                        </span>
                    </h4>
                </div>
            </div>

            <div class="col">
                <!-- cards -->
                <Info />
            </div>
        </div>
    </div>
</template>

<script>
import Info from '@/components/page5/Info'
export default {
    components: {
        Info
    },
    data: () => ({
        pasos: [
            {
                name: 'Definicíon',
                page: 1
            },
            {
                name: 'Especialidad',
                page: 2
            },
            {
                name: 'Adicionales',
                page: 3
            },
              {
                name: 'Condiciones',
                page: 4
            }
        ]
    })
}
</script>

<style scoped>
.step {
    width: 35px;
    height: 35px;
    display: flex;
    padding-left: 10px;
    border-radius: 50%;
    align-items: center;
    background-color: #00a2c2;
}
.top {
    padding-top: 140px;
}
</style>