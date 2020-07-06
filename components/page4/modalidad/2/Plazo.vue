<template>
    <div class="row">
        <div class="col">
            <div class="mt-5">
                <p class="size">Plazo Estimado:</p>
                <P>Indica el tiempo aproximado en el que necesitarás que se repita tu proyecto. Luego podrás precisarlo o revisarlo con mayor exactitud.</P>
            </div> 
            <!-- cards -->
                <div class="text-center card-group card-deck">
                    <div class="card">
                        <button
                            class="btn carta shadow tam"
                            @click="activar"
                        >
                            <div class="card-title">
                                <h5>1 a 7 Días</h5>
                            </div>
                        </button>
                    </div>
                    <div class="card">
                        <button class="btn btn carta shadow tam" @click="activar">
                            <div class="card-title">
                            <h5>8 a30 días</h5>
                            </div>
                        </button>
                    </div>
                    <div class="card">
                        <button class="btn btn carta shadow tam" @click="activar">
                            <div class="card-title">
                            <h5>Más de 30 días</h5>
                            </div>
                        </button>
                    </div>

                </div>

                <Rango />

                <div class="d-flex justify-content-between mb-5">
                    <nuxt-link to="/page3">
                        <button type="button" class="my-5 btn btn-link" style="color: #00a2c2;">Atras</button>
                    </nuxt-link>
                    <nuxt-link to="/page5_a">
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
.tam {
    height: 50px;
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
  padding: 16px 32px;
  text-align: center;
  text-decoration: none;
}
</style>