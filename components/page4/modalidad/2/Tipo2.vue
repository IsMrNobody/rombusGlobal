<template>
    <div class="row">
        <div class="col">
            <div class="mt-5 col-6">
                <p class="size">Tipo de proyecto:</p>
            </div> 
            <!-- cards -->
                <div class="text-center card-group card-deck">
                    <div class="card">
                        <button
                            class="btn carta shadow tam"
                            @click="activar"
                        >
                            <div class="card-title">
                                <img src="/icons/calendar.svg" height="30" alt="foto" class="mr-auto my-2">
                                <h5>Proyecto Único, empieza y termina una sola vez</h5>
                            </div>
                        </button>
                    </div>
                    <div class="card">
                        <button class="btn btn carta shadow tam" @click="activar">
                            <div class="card-title">
                                <img src="/icons/file.svg" height="30" alt="foto" class="mr-auto my-2">
                                <h5>Proyecto recurrente, se repite según plazo estimado</h5>
                            </div>
                        </button>
                    </div>
                    <div class="card">
                        <button class="btn btn carta shadow tam" @click="activar">
                            <div class="card-title">
                                <img src="/icons/question.svg" height="30" alt="foto" class="mr-auto my-2">
                                <h5>No lo sé aún lo definire luego</h5>
                            </div>
                        </button>
                    </div>
                </div>

                <Plazo v-if="mostrar" />                
                
        </div>
    </div>
</template>

<script>
import Plazo from '@/components/page4/modalidad/2/Plazo'
export default {
    components: {
        Plazo
    },
    data: () => ({
            mostrar: false
        }),
        methods: {
            activar() {
                this.mostrar = true
            }
        }
    }
</script>

<style scoped>
.tam{    
    height: 180px;
}
.carta:focus{
    color: white;
    background: #00a2c2;
}
p {
    font-size: 18px;
}
.size {
    font-size: 24px;
}
</style>