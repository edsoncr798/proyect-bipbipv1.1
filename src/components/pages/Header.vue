<script lang="ts" setup>
import { ref } from "vue";

const isLogin = ref(false);
</script>

<template>
  <!--! quitar el min-width  y agregar un max-width -->
  <header class="w-full absolute z-10 h-16">
    <div
      class="justify-between w-4/5 max-w-[1920px] items-center flex h-full mx-auto"
    >
      <i
        class="lg:order-1 block lg:hidden fa-sharp fa-solid fa-bars fa-beat"
      ></i>
      <!--? quiero que este div sea responsivo, pantalla grande tenga de width 450px y
            pantalla pequeña que tenga de width 200px  -->
      <div
        class="flex w-[160px] sm:w-[200px] md:w-[450px] lg:justify-between justify-center items-center"
      >
        <div class="h-[38px] w-[126px] z-50">
          <img
            class="w-full h-full"
            src="../../../images/logo-bip.svg"
            alt=""
          />
        </div>
        <div class="hidden lg:block">
          <button
            class="truncate hover:scale-105 transition duration-200 ease-in-out"
          >
            Sobre Nosotros
          </button>
          <button
            class="truncate hover:scale-105 transition duration-200 ease-in-out"
          >
            Contáctenos
          </button>
          <!-- <button class=" py-2 px-4 rounded overflow-hidden">
                        <span class="relative inline-block">
                          <span class="absolute inset-0 bg-white animate-loading"></span>
                          <span class="relative">Contáctenos</span>
                        </span>
                    </button> -->
        </div>
      </div>

      <!--! para pantalla desde 990px a mas...  -->
      <div class="hidden lg:block">
        <div class="w-[280px] flex justify-between">
          <button
            class="hover:text-white hover:bg-btn-hover hover:shadow-lg bg-white truncate font-medium"
          >
            Iniciar Sesión
          </button>
          <button
            class="hover:text-white hover:bg-btn-hover hover:shadow-lg bg-white truncate font-medium"
          >
            Registrarse
          </button>
        </div>
      </div>

      <!--! Para pantalla hasta los 991px  -->
      <i class="block lg:hidden fa-solid fa-circle-user text-3xl"></i>
      <!-- <img class="w-[55px] h-[55px] rounded-full" src="../../../images/user2.jpeg" alt="photo user"> -->
    </div>
  </header>
</template>

<style>
header {
  background: rgba(255, 255, 255, 0.4);
  box-shadow: 4px 7px 15px rgba(0, 0, 0, 0.08),
    inset -5px 5px 12px rgba(255, 255, 255, 0.05);
  backdrop-filter: blur(15px);
}

.animate-loading {
  animation: loading 1s ease-in-out infinite;
}

@keyframes loading {
  0% {
    left: -100%;
  }
  100% {
    left: 100%;
  }
}

.hover\:animate-loading:hover {
  animation-name: loading;
  animation-duration: 1s;
  animation-timing-function: ease-in-out;
  animation-iteration-count: infinite;
}
</style>
