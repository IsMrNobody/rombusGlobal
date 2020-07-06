<template>
    <div>
        <div class="mt-5">
          <h2>Cuéntanos de qué se trata tu proyecto</h2>
          <P>¡Explica brevemente en qué consiste tu necesidad y en 4 pasos tendras tu plan a tu medida!</P>

          <!-- Agregar titulo -->
          <div class="form-group flex-nowrap mt-5">
            <label>Ponle un título fácil, que identifique tu requerimiento *</label>
            <input type="text" class="form-control" placeholder="Título del proyecto (Ej: ...)">
          </div>

          <!-- Agregar parrafo -->
          <div class="mt-5">
            <p>Agrega un párrafo que nos ayude a entender lo que necesitas o el objetivo que desees lograr.*</p>
            <textarea 
              class="form-control" 
              id="textarea1" 
              rows="12" 
              placeholder="Descripción del proyecto">
            </textarea>
            <small id="textarea1" class="form-text text-muted">* Obligatorio</small>
          </div>
        </div>

        <!-- boton continuar -->
        <div class="d-flex justify-content-end mb-5">
          <nuxt-link to="page2">
            <button 
              type="button" 
              class="button btn btn-outline-dark my-5 btn-lg" 
              style="background-color: #00a2c2;">Continuar</button>
          </nuxt-link>
        </div>
    </div>
</template>

<style>
.button {
  width: 300px;
  color: white;
  font-size: 24px;
  cursor: pointer;
  padding: 16px 32px;
  text-align: center;
  text-decoration: none;
}
</style>