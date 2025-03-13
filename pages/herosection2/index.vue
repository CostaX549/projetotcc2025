<template>
    <nav class="navbar navbar-expand-lg bg-light shadow-sm">
      <div class="container">
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav mx-auto gap-4">
            <li class="nav-item"><NuxtLink class="nav-link " to="/"><h3 class="fw-bolder">Início</h3></NuxtLink></li>
            <li class="nav-item"><NuxtLink class="nav-link" to="/cadastrar"><h3 class="fw-bolder">Cadastrar</h3></NuxtLink></li>
            <li class="nav-item"><NuxtLink class="nav-link " to="/anonimo"><h3 class="fw-bolder ">Entrar anônimo</h3></NuxtLink></li>
          </ul>
        <div class="social-icons d-flex align-items-center justify-content-center">
            <a href="#" ><Icon name="logos:instagram-icon"   size="30"/></a>
            <a href="#"><Icon name="logos:whatsapp-icon" size="35" style="margin-top:2px; margin-left: 2px;" /></a>
  <a href="#" ><Icon name="logos:tiktok-icon"  size="31" style="margin-bottom: 1px;" /></a>


</div>
        </div>
      </div>
    </nav>
  
    <section class="hero d-flex align-items-center">
  <div class="hero-overlay"></div>

    <div class="row  hero-content position-absolute   " style="bottom: 25%; left: 15%;">
        <div class="d-flex flex-column align-items-center">
        <h1 class="fw-bold display-2 ">ConectaMente</h1>
        <p class="fs-4 bg-success text-white px-5  py-1  text-center" >
          Seu psicólogo a um click de distância
        </p>
    </div>

  </div>
</section>
<section class="custom-section">
    <div class="container">
        <div class="row align-items-center">
            <!-- Imagem -->
            <div class="col-md-6 text-center">
                <img src="~/assets/img/mulherlendo.jpg" alt="Mulher lendo" class="img-fluid rounded">
            </div>

            <div class="col-12 col-md-1 d-flex justify-content-center">
                <!-- Divisor Vertical no Desktop, Horizontal no Mobile -->
                <div class="border-start border-5 border-white d-none d-md-block" style="height: 400px;"></div>
                <div class="border-top border-5 border-white d-md-none mt-4" style="width: 100%; height: 6px;"></div>
            </div>
            
            <!-- Texto -->
            <div class="col-md-5">
                <div class="text-box">
                    <p class="fw-bold fs-4 text-justify">
                        A saúde mental é crucial para o bem-estar geral, afetando emoções, pensamentos e comportamentos. Cuidar dela melhora a qualidade de vida, ajuda a enfrentar desafios e fortalece relacionamentos. Conscientizar sobre sua importância contribui para a prevenção de doenças e quebra estigmas, incentivando a busca por ajuda.
                    </p>
                </div>
            </div>
        </div>
    </div>
</section>
</template>
<style scoped>
.hero {
    position: relative;
    background: url('~/assets/img/hero-img-4.webp') no-repeat center center/cover;
    height: 95vh;
    color: white;
}
.social-icons a {
    margin: 0 10px;
    font-size: 24px;
}

.instagram {
    color: #E4405F; /* Cor do Instagram */
}
.whatsapp {
    color: #25D366; /* Cor do WhatsApp */
}
.tiktok {
    color: #69C9D0; /* Cor do TikTok */
}
.hero-overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.4);
}
.hero-content {
    color: black;
}

h3 {
    color: black;
}

.custom-section {
    background-color: #A5B98E; /* Verde similar ao da imagem */
    padding: 40px 0;
}

.text-box {
    background-color: #A5B98E;
 
    color: black;
}

@media (max-width: 900px) {
    .custom-section {
        padding: 20px 0;
    }

    .text-box {
        padding: 15px;
    }

    .border-top {
        height: 4px;
    }

    .col-md-6, .col-md-5 {
        width: 100%;
        margin-bottom: 20px;
    }
}
</style>