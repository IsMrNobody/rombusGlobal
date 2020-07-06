<template>
    <div>
        <div class="mt-5">
          <h2>Agrega información valiosa</h2>
          <P>Puedes adjuntar un archivo o imagen que describa tu proyecto o un ejemplo de referencia.</P>

          <!-- Agregar archivo -->
          <div 
            class="card text-center d-flex justify-content-center borde"
            style="height: 400px;"
          > 
              <img
                src="/icons/solid-file.svg" 
                class="imag mb-2"
                >
                <p>Nombre del archivo</p>
            <div class="custom-file">
              <input 
                type="file"
                class="custom-file-input"
              >
               <label 
                class="custom-file-label"
               >
                <h4>
                  Arrastra o sube un archivo o imagen(jpg, png, pdf, doc)
                </h4>
               </label>
            </div>
          </div>

          <!-- Agregar parrafo -->
          <div 
            class="mt-5">
            <p>
              Tu comentario (ideas, pedidos, ejemplos, webs, paleta de colores, marcas preferidas, versiones previas, etc.):
            </p>

            <textarea 
              class="form-control" 
              id="textarea1" 
              rows="12" 
              placeholder="Descripción del proyecto">
            </textarea>

            <small 
              id="textarea1"
              class="form-text text-muted"
            >
              * Obligatorio
            </small>
          </div>
        </div>

        <!-- boton continuar -->
        <div
          class="d-flex justify-content-between mb-5">
          <nuxt-link to="/page2">
            <button 
              type="button" 
              class="my-5 btn btn-link" 
              style="color: #00a2c2;"
            >
              Atras
            </button>
          </nuxt-link>

          <nuxt-link to="page4">
            <button 
              type="button"
              class="button btn btn-outline-dark my-5 btn-lg" style="background-color: #00a2c2;"
            >
              Continuar
            </button>
          </nuxt-link>

        </div>
    </div>
</template>

<style>
.button {
  border: none;
  width: 300px;
  color: white;
  font-size: 24px;
  margin: 4px 2px;
  cursor: pointer;
  padding: 16px 32px;
  text-align: center;
  text-decoration: none;
}
.borde {
  border-width: 6px;
  border-style: dashed;
  border-color: #00a2c2;
}
.texto {
  align-self: center;
}
p {
  font-size: 20px;
}
.imag {
  width: 80px;
  align-self: center;
}
</style>
