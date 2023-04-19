<script lang="ts" setup>
import HowFunctionMobile from ".././shared/HowFunctionMobile.vue";
import HowFunctionDesktop from "../shared/HowFunctionDesktop.vue";
</script>
<template>
  <section
    class="bg-[#FFFFFF] pb-[30px] w-full flex flex-col items-center rounded-[22px]"
  >
    <h1
      class="not-italic text-[#0D47A1] text-center leading-[70px] md:leading-[141px] font-medium text-[26px] md:text-[46px] lg:text-[70px]"
    >
      ¿Como funciona?
    </h1>
    <article class="w-full px-[20px] md:flex md:justify-center ">
      <HowFunctionMobile class="block md:hidden" />
      <HowFunctionDesktop class="hidden md:block"/>
    </article>
  </section>
</template>
