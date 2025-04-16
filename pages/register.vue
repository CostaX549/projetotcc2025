<template>

<section class="vh-100" style="background-color: #77DD77;">
<ul class="nav nav-tabs nav-fill mb-3" id="ex1" role="tablist">
  <li class="nav-item" role="presentation">
    <a
      data-mdb-tab-init
      class="nav-link active"
      id="ex2-tab-1"
      href="#ex2-tabs-1"
      role="tab"
      aria-controls="ex2-tabs-1"
      aria-selected="true"
      >Criar Conta Pessoal</a
    >
  </li>
  <li class="nav-item" role="presentation">
    <a
      data-mdb-tab-init
      class="nav-link"
      id="ex2-tab-2"
      href="#ex2-tabs-2"
      role="tab"
      aria-controls="ex2-tabs-2"
      aria-selected="false"
      >Criar conta profissional</a
    >
  </li>
 
</ul>
<!-- Tabs navs -->

<!-- Tabs content -->
<div class="tab-content" id="ex2-content">
  <div
    class="tab-pane fade show active"
    id="ex2-tabs-1"
    role="tabpanel"
    aria-labelledby="ex2-tab-1"
  >
  
    <div class="container h-100  pt-3">
      <div class="row d-flex justify-content-center align-items-center ">
      <div class="col col-xl-10">
        <div class="card" style="border-radius: 1rem;">
          <div class="row g-0">
            <div class="col-md-6 col-lg-5 d-none d-md-block">
              <img src="~/assets/img/psicologa.jpg"
                alt="login form" class="img-fluid" style="border-radius: 1rem 0 0 1rem;" />
            </div>
            <div class="col-md-6 col-lg-7 d-flex align-items-center">
              <div class="card-body p-4 p-lg-5 text-black">

                <form>

                  <div class="d-flex align-items-center mb-3 pb-1">
                
                    <span class="h1 fw-bold mb-0">Crie sua conta</span>
                  </div>

                  <h5 class="fw-normal mb-3 pb-3" style="letter-spacing: 1px;">Faça registro da sua conta</h5>
                  <div data-mdb-input-init class="form-outline mb-4">
                    <input type="text" id="form2Example17" class="form-control form-control-lg" />
                    <label class="form-label" for="form2Example17">Nome</label>
                  </div>
                  <div data-mdb-input-init class="form-outline mb-4">
                    <input type="email" id="form2Example17" class="form-control form-control-lg" />
                    <label class="form-label" for="form2Example17">Email</label>
                  </div>
                  <div data-mdb-input-init class="form-outline mb-4">
                    <input type="password" id="form2Example27" class="form-control form-control-lg" />
                    <label class="form-label" for="form2Example27">Senha</label>
                  </div>
                  <div data-mdb-input-init class="form-outline mb-4">
                    <input type="password" id="form2Example27" class="form-control form-control-lg" />
                    <label class="form-label" for="form2Example27">Confirmar Senha</label>
                  </div>

                  <div class="pt-1 mb-4">
                    <button data-mdb-button-init data-mdb-ripple-init class="btn text-white btn-lg btn-block"  type="button"  style="background-color: #77DD77;">Registrar</button>
                  </div>


                  <p class="mb-5 pb-lg-2" style="color: #393f81;">Já possui uma conta? <NuxtLink href="/login" style="color: #77DD77;"
                      >Faça login aqui</NuxtLink></p>
                
                </form>

              </div>
            </div>
          </div>
        </div>
      </div>
 
    </div>
  </div>
  </div>
  <div
    class="tab-pane fade"
    id="ex2-tabs-2"
    role="tabpanel"
    aria-labelledby="ex2-tab-2"
  >
    Tab 2 content
  </div>

</div>
</section>

</template>
<style scoped>
.nav-tabs .nav-link.active {
  background-color: transparent; /* cor de fundo da aba ativa */
  color: white; /* texto verde (como seu bg-success) */
  border-color: #198754 #198754 #ffffff; /* bordas coloridas, exceto embaixo */
  font-weight: bold;
}
.nav-tabs .nav-link:hover {
  background-color: transparent;
  color: #ffffff;
}
</style>
<script setup lang="ts">
import { onMounted } from 'vue'
useHead({
  script: [
    {
      src: 'https://cdnjs.cloudflare.com/ajax/libs/mdb-ui-kit/6.4.2/mdb.min.js',
      integrity: 'sha512-kZKnID21//xaFiEISBXk6V1AdFCPOIpHhuEdBMprlAHdb0ICnvgSLsb89DAixlLJDuPyvNR+hN3lPvsFNn5XLg==',
      crossorigin: 'anonymous',
      defer: true,
      tagPosition: 'bodyClose',
    },
  ],
})

  onMounted(async () => {
    const { Tab, Input, Ripple, initMDB } = await import('mdb-ui-kit')
    initMDB({ Tab, Input, Ripple })
  })

</script>