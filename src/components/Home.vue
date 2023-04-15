<script lang="ts" setup>
import MenuToggleUsers from './shared/MenuToggleUsers.vue'
</script>

<template>
  <section class="home w-full flex h-full relavite items-center justify-center">
    <div class="mx-auto w-[670px]   absolute ">
      <h1 class=" text-white font-medium text-6xl leading-[70px]">
        Aprovecha los multiples <br> servicios con la mejor <br> solución
      </h1>
      <div class="flex mt-10">
        <button class="w-[192.68px] mr-5 h-[60px]">
          <img
            class="rounded-[15px] w-full h-full"
            src="../../images/app+store2.jpeg"
            alt=""
          />
        </button>
        <button class="w-[192.68px] h-[60px]">
          <img
            class="rounded-[15px] w-full h-full"
            src="../../images/image.jpeg"
            alt=""
          />
        </button>
      </div>
    </div>
    <MenuToggleUsers class="hidden" />
  </section>
</template>

<style>
.home {
  background-image: linear-gradient(135deg, #2458b898 10%, #151a7b4b 90%),
    url(".././.././images/photo-home.jpg");
  background-size: 100% 100%;
  background-repeat: no-repeat;
}

.home div h1{
    font-family: Baloo Bhaina 2;
    
}
</style>
