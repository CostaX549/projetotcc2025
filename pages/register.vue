<template>


<section class="vh-100 bg-success" >
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
  
    <div class="container h-100 pt-5">
      <div class="row d-flex justify-content-center align-items-center h-100">
        <div class="col-12 col-md-9 col-lg-7 col-xl-6">
          <div class="card" style="border-radius: 15px;">
            <div class="card-body p-5">
              <h2 class="text-uppercase text-center mb-5">Criar conta</h2>

              <form>

                <div data-mdb-input-init class="form-outline mb-4">
                  <input type="text" id="form3Example1cg" class="form-control form-control-lg" />
                  <label class="form-label" for="form3Example1cg">Nome</label>
                </div>

                <div data-mdb-input-init class="form-outline mb-4">
                  <input type="email" id="form3Example3cg" class="form-control form-control-lg" />
                  <label class="form-label" for="form3Example3cg">Email</label>
                </div>

                <div data-mdb-input-init class="form-outline mb-4">
                  <input type="password" id="form3Example4cg" class="form-control form-control-lg" />
                  <label class="form-label" for="form3Example4cg">Senha</label>
                </div>

                <div data-mdb-input-init class="form-outline mb-4">
                  <input type="password" id="form3Example4cdg" class="form-control form-control-lg" />
                  <label class="form-label" for="form3Example4cdg">Confirmar Senha</label>
                </div>

              
                <div class="d-flex flex-column gap-2 justify-content-center">
                  <button  type="button" data-mdb-button-init
                    data-mdb-ripple-init class="btn btn-success btn-block btn-lg gradient-custom-4 text-white">Registrar</button>
                    <button data-mdb-button-init data-mdb-ripple-init class="btn btn-lg btn-block btn-primary" style="background-color: #dd4b39;"
                    type="submit"><i class="fab fa-google me-2"></i> Continuar com Google</button>
                </div>
              
                <p class="text-center text-muted mt-5 mb-0">Have already an account? <a href="#!"
                    class="fw-bold text-body"><u>Login here</u></a></p>

              </form>

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