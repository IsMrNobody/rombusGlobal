<template>
    <div class="">
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
                        <button class="btn btn carta shadow tam" @click="activar2">
                            <div class="card-title">
                               <img src="/icons/file.svg" height="30" alt="foto" class="mr-auto my-2">
                                <h5>Proyecto recurrente, se repite según plazo estimado</h5>
                            </div>
                        </button>
                    </div>
                    <div class="card">
                        <button class="btn btn carta shadow tam" @click="activar3">
                            <div class="card-title">
                                <img src="/icons/question.svg" height="30" alt="foto" class="mr-auto my-2">
                                <h5>No lo sé aún lo definire luego</h5>
                            </div>
                        </button>
                    </div>
                </div>

                <Rango />

                <div class="d-flex justify-content-between mb-5">
                    <nuxt-link to="/page3">
                        <button type="button" class="my-5 btn btn-link" style="color: #00a2c2;">Atras</button>
                    </nuxt-link>
                    <nuxt-link to="/page5">
                        <button type="button" class="button btn btn-outline-dark my-5 btn-lg" style="background-color: #00a2c2;">¡Terminado! Ir a Resúmen</button>
                    </nuxt-link>
                </div>                
        </div>
    </div>
</template>

<script>
import Rango from '@/components/page4/modalidad/Rango'
export default {
    components: {
        Rango
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
.button {
  border: none;
  width: 360px;
  color: white;
  font-size: 24px;
  margin: 4px 2px;
  cursor: pointer;
  text-align: center;
  padding: 16px 32px;
  text-decoration: none;
}
</style>