<template>
  <div class="col">

    <!-- barra De Navegación -->
    <nav
      class="nav navbar navbar-expand-lg navbar-dark"  style="background-color: #123a40;"
    > 
    <!-- logo -->
      <div class="col">
        <a href="/" class="ml-5 mx-5 navbar-brand">
          <img src="/rg-logo.svg" height="80" alt="foto" >
        </a>
      </div>

       <!-- direcciones -->
       <div class="justify-content-end" id="navbar">
          <ul class="navbar-nav mt-2 mr-auto text-uppercase">
            <li class="nav-item active">
              <a class="nav-link" href="#">Soluciones</a>
            </li>
            <li class="nav-item active">
              <a class="nav-link" href="#">Staff</a>
            </li>
            <li class="nav-item active">
              <a class="nav-link" href="#">Blog</a>
            </li>
          </ul>
        </div>
        

        <!-- boton -->
        <div class="mr-5">
          <button 
            class="btn my-2 my-sm-0 btn-lg ml-4 border border-white text-uppercase bor" style="background-color: #24a4b4; color: white;" type="submit">Publicar proyecto</button>

          <!-- foto avatar -->
          <img 
            width="50" 
            height="50" 
            src="/perfil.jpg" 
            class="rounded-circle mx-3"
          >
        </div>
    </nav>
  </div>
</template>

<style>
.bor {
  border-radius: 25px;
}
</style>
