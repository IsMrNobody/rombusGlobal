<template>
    <div>
         <!-- boton continuar -->
        <div class="d-flex justify-content-between mb-5">
            <div class="mt-5 mb-5">
                <h2 class="mt-3">Resumen del proyecto</h2>
            </div>
            <nuxt-link to="/">
                <button 
                    type="button"
                    style="background-color: #f39a18;"
                    class="button btn btn-outline-dark my-5">¡Enviar Ahora!
                </button>
            </nuxt-link>
        </div>

        <!-- cards -->
        <div class="card-body shadow">
            <h5 class="card-title">Va título Modelo 3D de un tanque o fusil</h5>
            <p>
                Va definición El objetivo de lograr empresas verdes trata de un cambio cultural, una toma de conciencia 
                que como de conciencia que como ciudadanos. RombusDATA Blog: El objetiv</p>
        </div>
        <!-- categorias -->
        <div class="card mt-2">

            <div class="card-body mt-1 fondo">
                <h5 class="card-title">Diseño y Creatividad</h5>
            </div>

            <div class=" card-body mt-1 fondo">
                <h5 class="card-title">Diseño de Aplicación / IOS</h5>
            </div>

        </div>
            <div class="card-body shadow mt-2">
                <p>
                    Va comentario RombusDATA Blog: El objetivo de lograr empresas verdes trata de un cambio cultural, una 
                    toma de conciencia que como ciudadanos.</p>
            </div>
        
        <!-- archivo en adjunto -->
        <div class="mt-2 mb-2 btn btn-link">
            <h4>Adjunto Archivo</h4>
        </div>

        <!-- cards -->
        <div class="card-group card-deck mt-4">
            <div class="card">
                <h5>Con quien prefieres resolver el trabajo:</h5>
                <button class="btn carta shadow tam">
                    <div class="card-title">                    
                    <img src="/icons/map.svg" height="30" alt="foto" class="mr-auto my-1">
                    <i class="fa fa-car"></i>
                    <h5>
                        Rombus Ciudad
                        cercano a mi ubicación</h5>
                    </div>
                </button>
            </div>

            <div class="card">
                <h5>Tipo de proyecto:</h5>
                <button class="btn carta shadow tam">
                    <div class="card-title">                    
                        <img 
                            src="/icons/question.svg" 
                            height="30" alt="foto" 
                            class="mr-auto my-1">
                        <h5>No lo sé aún, lo definiré luego</h5>
                    </div>
                </button>
            </div>
        </div>

        <!-- datos de usuario -->
        <div class="col-8 mt-4">
            <h5>Datos de contacto y ubicación del proyecto:</h5>
            <div class="form-row">
                <div class="col-md-6">
                    <p>Juan Carlos Pepe</p>
                </div>

                <div class="col-md-6">
                    <p>juanpepe@empresa.com</p>
                </div>

                <div class="col-md-6">
                    <p>541112345678</p>
                </div>

                <div class="col-md-6">
                    <p>Buenos Aires, Argentina</p>
                </div>
            </div>
        </div>

        <!-- rango de precio -->
        <div class="d-flex justify-content-end mt-5">
            <div class="form-group">
                <label>Tu presupuesto</label>
                <input 
                type="number" 
                class="form-control form-control-lg" 
                id="Input" 
                placeholder="$ 1.900">
            </div>
        </div>


        <!-- botones final -->
        <div class="row d-flex justify-content-around mb-5 mt-4">
            <div>
                <button class="btn btn-secondary button">Guardar borrador</button>
                <button class="btn btn-dark button">Cerrar proyecto</button>
            </div>
            <div>
                <button class="btn btn-outline-dark button" style="background-color: #f39a18;">¡Enviar Ahora!</button>
            </div>
        </div>
    </div>
</template>

<style scoped>
.tam{    
    height: 200px;
}
p {
    font-size: 18px;
}
.carta:focus{
    color: white;
    background: #00a2c2;
}
.button {
  height: 70px;
  color: white;
  font-size: 24px;
  cursor: pointer;
}
.fondo {
    background-color: #f39a18;
}
</style>