<script lang="ts" setup>
import MenuToggleUsers from "./shared/MenuToggleUsers.vue";
import BestOption from "./sections/BestOption.vue";
import HowFunction from "./sections/HowFunction.vue";
import MakeACall from "./sections/MakeACall.vue";
import JoinUs from "./sections/JoinUs.vue";
import Warranty from "./sections/Warranty.vue";
import StartNow from "./sections/StartNow.vue";
</script>
<template>
  <section class="home w-full flex h-screen items-center">
    <div class="ml-[15%]">
      <h1
        class="text-[#FFFFFF] not-italic text-[25px] md:text-[60px] md:font-medium md:leading-[60px]"
      >
        Aprovecha los multiples <br />
        servicios con la mejor <br />
        solución
      </h1>
      <div class="home-btn md:mt-10">
        <button class="w-[120px] md:w-[192.68px] md:mr-5 md:h-[60px]">
          <img
            class="rounded-[5px] md:rounded-[15px] w-full h-full"
            src="../../images/app+store2.jpeg"
            alt=""
          />
        </button>
        <button class="w-[120px] md:w-[192.68px] md:h-[60px]">
          <img
            class="rounded-[5px] md:rounded-[15px] w-full h-full"
            src="../../images/image.jpeg"
            alt=""
          />
        </button>
      </div>
    </div>
    <MenuToggleUsers class="hidden" />
  </section>
  <BestOption />
  <HowFunction />
  <MakeACall />
  <JoinUs />
  <Warranty />
  <StartNow />
</template>

<style>
.home {
  background-image: linear-gradient(135deg, #2458b898 10%, #151a7b4b 90%),
    url(".././.././images/photo-home1.jpg");
  background-size: 100% 100%;
  background-repeat: no-repeat;
}

@media (max-width: 769px) {
  .home div .home-btn {
    display: flex;
    flex-direction: column;
    margin-top: 20px;
  }

  .home div .home-btn button {
    margin-top: 5px;
  }
}

@media (min-width: 990px) {
  .home {
    background-image: linear-gradient(135deg, #2458b898 10%, #151a7b4b 90%),
      url(".././.././images/photo-home.jpg");
    background-size: 100% 100%;
    background-repeat: no-repeat;
    min-width: 500px;
    min-height: 500px;
  }
}
</style>
