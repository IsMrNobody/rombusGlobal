<template>
    <div class="row">
        <div class="col">
            <div class="mt-5 col-6">
                <p class="size">Selecciona el nivel de experiencia</p>
                <P>Inicial >> talentos que transitan sus primeros años.</P>
                <P>Medio >> ya cuentan con experiencia comprobable.</P>
                <P>Experto >> poseen total dominio de la materia.</P>
            </div> 
            <!-- cards -->
                <div class="text-center card-group card-deck">
                    <div class="card">
                        <button
                            class="btn carta shadow tam"
                            @click="activar"
                        >
                            <div class="card-title">
                                <h5>Inicial</h5>
                                <h5>$</h5>
                            </div>
                        </button>
                    </div>
                    <div class="card">
                        <button class="btn btn carta shadow tam" @click="activar">
                            <div class="card-title">
                            <h5>Medio</h5>
                            <h5>$$</h5>
                            </div>
                        </button>
                    </div>
                    <div class="card">
                        <button class="btn btn carta shadow tam" @click="activar">
                            <div class="card-title">
                            <h5>Experto</h5>
                            <h5>$$$</h5>
                            </div>
                        </button>
                    </div>

                </div>

            <Tipo v-if="mostrar" />
        </div>
    </div>
</template>

<script>
import Tipo from '@/components/page4/modalidad/1/Tipo'
export default {
    components: {
    Tipo
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