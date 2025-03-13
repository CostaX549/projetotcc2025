<template>
  <nav class="navbar fixed-top navbar-expand-lg bg-body-tertiary">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">ConectaMente</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">Início</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Sobre Nós</a>
          </li>
          <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              Cadastrar
            </a>
            <ul class="dropdown-menu">
              <li><a class="dropdown-item" href="#">Entrar</a></li>
              <li><a class="dropdown-item" href="#">Registrar</a></li>
              <li><hr class="dropdown-divider"></li>
              <li><a class="dropdown-item" href="#">Entrar Anônimo</a></li>
            </ul>
          </li>
         <!--  <li class="nav-item">
            <a class="nav-link disabled" aria-disabled="true">Disabled</a>
          </li> -->
        </ul>
        <div class="social-icons d-flex align-items-center justify-content-center">
            <a href="#" ><Icon name="logos:instagram-icon"   size="25"/></a>
            <a href="#"><Icon name="logos:whatsapp-icon" size="30" style="margin-top:2px; margin-left: 2px;" /></a>
  <a href="#" ><Icon name="logos:tiktok-icon"  size="25" style="margin-bottom: 1px;" /></a>


</div>
      </div>
    </div>
  </nav>
  <section class="bg-success">
    <div class="container-fluid overflow-hidden">
      <div class="row">
        <div class="col-12 col-md-6 order-1 order-md-0 align-self-md-end">
          <div class="row py-3 py-sm-5 py-xl-9 mt-md-10 justify-content-sm-center d-flex">
            <div class="col-12 col-sm-10">
              <h2 class="display-2 fw-bolder mb-4 text-white">ConectaMente</h2>
              <div class="row">
                <div class="col-12 col-xxl-8">
                  <p class="fs-5 mb-5 text-white">Encontre equilíbrio e bem-estar emocional com nossos recursos e conteúdos exclusivos. No ConectaMente, ajudamos você a desenvolver sua melhor versão através de orientação, apoio e técnicas de autoajuda.</p>
                </div>
              </div>
              <div class="d-grid gap-2 d-sm-flex">
                <button type="button" class="btn btn-warning bsb-btn-2xl rounded-pill">Comece Agora</button>
              </div>
            </div>
          </div>
        </div>
        <div class="col-12 col-md-6 p-0">
          <img class="img-fluid object-fit-cover w-100" style="max-height: 90vh;" loading="lazy" src="~/assets/img/hero-img-1.png" alt="Encontre equilíbrio e bem-estar emocional">
        </div>
      </div>
    </div>
  </section>
  
  </template>
  
  <script>
  </script>

  <style>
  .social-icons a {
    margin: 0 10px;
    font-size: 24px;
}
</style>
  