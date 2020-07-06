<template>
    <div>
        <div class="d-flex flex-wrap">
            <div class="mt-5 col">
                <p class="size">Atención localizada</p>
                <p>Un Profesional de Rombus, cercano en tu localidad, se contactará para atender y gestionar personalmente las necesidades del proyecto.</p>
            </div>
            <div class="mt-5 col">
                <p class="size">Completa los datos de contacto y ubicación de tu proyecto:</p>

                <div class="form-row">
                    <div class="col-md-6 mb-3">
                        <input type="text" class="form-control form-control-sm" value="Jusan Carlos" required>
                    </div>

                    <div class="col-md-6 mb-3">
                        <input type="text" class="form-control form-control-sm" value="Pepe" required>
                    </div>

                    <div class="col-md-6 mb-3">
                        <input type="text" class="form-control form-control-sm" value="juanpepe@empresa.com" required>
                    </div>

                    <div class="col-md-6 mb-3">
                        <input type="text" class="form-control form-control-sm" value="Whatsapp" required>
                    </div>

                    <div class="col-md-6 mb-3">
                        <input type="text" class="form-control form-control-sm" value="Ciudad" required>
                    </div>

                    <div class="col-md-6 mb-3">
                        <input type="text" class="form-control form-control-sm" value="Pais" required>
                    </div>
                </div>

                <Rango />

            </div>
        </div>
        <div class="d-flex justify-content-between mb-5">
            <nuxt-link to="/page3">
                <button type="button" class="my-5 btn btn-link" style="color: #00a2c2;">Atras</button>
            </nuxt-link>
            <nuxt-link to="/page5_b">
                <button type="button" class="button btn btn-outline-dark my-5 btn-lg" style="background-color: #00a2c2;">¡Terminado! Ir a Resúmen</button>
            </nuxt-link>
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
.size {
    font-size: 18px;
}
.button {
  border: none;
  width: 360px;
  color: white;
  cursor: pointer;
  font-size: 24px;
  margin: 4px 2px;
  padding: 16px 32px;
  text-align: center;
  text-decoration: none;
}
</style>