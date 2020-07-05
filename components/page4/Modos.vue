<template>
    <div>
        <div class="mt-5 mb-5">
            <h2>Selecciona el area profesional adecuada</h2>
            <P>Elige el servicio que enfoca tu necesidad principal:</P>
        </div>

        <!-- cards -->
        <div class="card-group card-deck">
            <div class="card">
                <button class="btn carta shadow tam" @click="activar">
                    <div class="card-title">                    
                    <img src="/icons/user.svg" height="30" alt="foto" class="mr-auto my-1">
                    <i class="fa fa-car"></i>
                    <h5>Un profesional individual</h5>
                    </div>
                </button>
            </div>
            <div class="card">
                <button class="btn btn carta shadow tam" @click="activar2">
                    <i class="fas fa-camera"></i>
                    <div class="card-title">
                    <img src="/icons/users.svg" height="30" alt="foto" class="mr-auto my-1">
                    <h5>Proyect manager y equipo</h5>
                    </div>
                </button>
            </div>
            <div class="card">
                <button class="btn btn carta shadow tam" @click="activar3">
                    <div class="card-title">
                    <img src="/icons/map.svg" height="30" alt="foto" class="mr-auto my-1">
                    <h5>Rombus Ciudad / cercana a mi hubicación</h5>
                    </div>
                </button>
            </div>
            <div class="card">
                <button class="btn btn carta shadow tam" @click="activar4">
                    <div class="card-title">
                    <img src="/icons/building.svg" height="30" alt="foto" class="mr-auto my-1">
                    <h5>Rombus Central / atención corporativa</h5>
                    </div>
                </button>
            </div>

        </div>

        <Expe v-if="mostrar" />
        <Tipo2 v-if="mostrar2" />
        <Tipo3 v-if="mostrar3" />
        <Tipo4 v-if="mostrar4" />

        <!-- boton continuar -->
        <div class="d-flex justify-content-between mb-5">
            <nuxt-link to="/page3">
                <button type="button" class="my-5 btn btn-link" style="color: #00a2c2;">Atras</button>
            </nuxt-link>
            <nuxt-link to="/page5">
                <button type="button" class="button btn btn-outline-dark my-5 btn-lg" style="background-color: #00a2c2;">¡Terminado! Ir a Resúmen</button>
            </nuxt-link>
        </div>
    </div>
</template>

<script>
import Expe from '@/components/page4/modalidad/1/Expe'
import Tipo2 from '@/components/page4/modalidad/2/Tipo2'
import Tipo3 from '@/components/page4/modalidad/3/Tipo3'
import Tipo4 from '@/components/page4/modalidad/4/Tipo4'
export default {
    components: {
        Expe,
        Tipo2,
        Tipo3,
        Tipo4
    },
    data: () => ({
        mostrar: false,
        mostrar2: false,
        mostrar3: false,
        mostrar4: false
    }),
    methods: {
        activar() {
            this.mostrar = true
            this.mostrar2 = false
            this.mostrar3 = false
            this.mostrar4 = false
        },
        activar2() {
            this.mostrar2 = true
            this.mostrar = false
            this.mostrar3 = false
            this.mostrar4 = false
        },
         activar3() {
             this.mostrar3 = true
            this.mostrar2 = false
            this.mostrar = false
            this.mostrar4 = false
        },
         activar4() {
            this.mostrar4 = true
            this.mostrar3 = false
            this.mostrar2 = false
            this.mostrar = false
        }
    }
}
</script>

<style scoped>
.tam{    
    height: 200px;
}
.carta:focus{
    background: #00a2c2;
    color: white;
}
p {
    font-size: 18px;
}
.button {
  border: none;
  color: white;
  padding: 16px 32px;
  text-align: center;
  text-decoration: none;
  font-size: 24px;
  margin: 4px 2px;
  cursor: pointer;
  width: 360px;
}
</style>