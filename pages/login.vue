<template>
<section class="vh-100 "  style="background-color: #77DD77;">
  <div class="container py-5 h-100">
    <div class="row d-flex justify-content-center align-items-center h-100">
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
                
                    <span class="h1 fw-bold mb-0">ConectaMente</span>
                  </div>

                  <h5 class="fw-normal mb-3 pb-3" style="letter-spacing: 1px;">Faça login na sua conta aqui</h5>

                  <div data-mdb-input-init class="form-outline mb-4">
                    <input type="email" id="form2Example17" class="form-control form-control-lg" />
                    <label class="form-label" for="form2Example17">Email</label>
                  </div>

                  <div data-mdb-input-init class="form-outline mb-4">
                    <input type="password" id="form2Example27" class="form-control form-control-lg" />
                    <label class="form-label" for="form2Example27">Senha</label>
                  </div>

                  <div class="pt-1 mb-4">
                    <button data-mdb-button-init data-mdb-ripple-init class="btn text-white  btn-lg btn-block"  style="background-color: #77DD77;" type="button">Login</button>
                  </div>

                  <a class="small text-muted" href="#!">Esqueceu a senha?</a>
                  <p class="mb-5 pb-lg-2" style="color: #393f81;">Não possui uma conta? <NuxtLink href="/register"  style="color: #77DD77;"
                      >Registre-se aqui</NuxtLink></p>
                
                </form>

              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>
</template>
<style scoped>
.cascading-right {
  margin-right: -50px;
}

@media (max-width: 991.98px) {
  .cascading-right {
    margin-right: 0;
  }
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
 
      tagPosition: 'bodyClose',
    },
  ],
})
onMounted(async () => {

    const mdb = await import('mdb-ui-kit')
    mdb.initMDB({ Input: mdb.Input })
 
})
</script>