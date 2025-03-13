<template>
    <div class="d-sm-flex align-items-center justify-content-between w-100" style="height: 100vh;">
      <div class="col-md-4  mb-4 mb-sm-0 headline position-relative  headline" >
        <span class="text-dark text-uppercase">Conectando Mentes</span>
        <h1 class="display-4 my-4 font-weight-bold">
          Conecta<span class="text-success">Mente</span>
        </h1>
        <a href="#" class="btn px-5 py-3 text-white mt-3 mt-sm-0 bg-success" style="border-radius: 30px; ">
          Começe Agora
        </a>
      </div>
      <!-- in mobile remove the clippath -->
      <div class="col-md-8 h-100 clipped bob" >
      </div>
    </div>
  </template>
  
  <style scoped>
 
  
  body {
    font-family: "Poppins", sans-serif !important;
  }
  


  .headline {
    left: 180px;
  }
  
  .clipped {
    clip-path: polygon(50% 0, 100% 0, 100% 100%, 0% 100%);
  }
  
  @media screen and (max-width: 650px) {
    .headline {
      left: 20px;
    } 
    .clipped {
      clip-path: none;
      max-height: 300px !important;
    }
  }

  .bob {
  min-height: 350px; background-image: url('~/assets/img/hero-img-4.webp'); background-position: center; background-size: cover;
  }
  </style>
  