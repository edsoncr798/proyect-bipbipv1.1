<script lang="ts" setup>
import { defineComponent, ref } from "vue";
import HowFunctionMobile from "./HowFunctionMobile.vue";

const isSelected = ref(false);

const isSelectedClicks = async () => {
  // isSelected.value = !isSelected.value;
  // console.log(isSelected.value);
};
</script>

<template>
  <div class="max-w-[1065px]">
    <div class="w-full flex">
      <div class="w-full pr-[60px]">

        <div class="flex" @click="isSelectedClicks">
          <div>
            <div
              :class="{ 'selected-step': isSelected }"
              class="w-[50px] h-[50px] md:w-[70px] md:h-[70px] rounded-[50%] bg-[#0D47A1]  text-[#FFFFFF] text-center text-[45px] font-medium md:font-semibold md:leading-[60px]"
            >
              1
            </div>
            <div
              :class="{ 'selected-step': isSelected }"
              class="w-[5px] h-[50px] lg:h-[100%] bg-[#0D47A1] mx-auto"
            ></div>
          </div>
          <div class="ml-5 md:ml-10 mt-[15px] md:mt-[0px]">
            <h2
              class="text-[#0D47A1] font-medium not-italic md:text-[30px] lg:text-[40px] lg:leading-[80px]"
            >
              Toca para reservar
            </h2>
            <p
              class="text-start not-italic font-normal text-[10px] md:text-[15px] lg:text-[22px] lg:leading-[30px]"
            >
              Solo levanta tu teléfono y colócalo donde quieras ir. La
              aplicación te convertirá en un conductor en poco tiempo.
            </p>
          </div>
        </div>

        <div class="flex" @click="isSelectedClicks">
          <div>
            <div
              :class="{ 'selected-step': isSelected }"
              class="w-[50px] h-[50px] md:w-[70px] md:h-[70px] rounded-[50%] bg-[#EAEAEA] border-2 border-[#D8D8D8] text-[#FFFFFF] text-center text-[45px] font-medium md:font-semibold md:leading-[60px]"
            >
              2
            </div>
            <div
              :class="{ 'selected-step': isSelected }"
              class="w-[5px] h-[100%] lg:h-[100%] bg-[#D8D8D8] mx-auto"
            ></div>
          </div>
          <div class="ml-5 md:ml-10 mt-[15px] md:mt-[0px]">
            <h2
              class="text-[#0D47A1] font-medium not-italic md:text-[30px] lg:text-[40px] lg:leading-[80px]"
            >
              Detalles de conductor
            </h2>
            <p
              class="text-start not-italic font-normal text-[10px] md:text-[15px] lg:text-[22px] lg:leading-[30px]"
            >
              Una vez que su solicitud de viaje es aceptada, la aplicación le
              notifica automáticamente todos los detalles del conductor,
              incluyendo el modelo y marca del automóvil.
            </p>
          </div>
        </div>

        <div class="flex">
          <div>
            <div
              class="w-[50px] h-[50px] md:w-[70px] md:h-[70px] rounded-[50%] bg-[#EAEAEA] border-2 border-[#D8D8D8] text-[#FFFFFF] text-center text-[45px] font-medium md:font-semibold md:leading-[60px]"
            >
              3
            </div>
            <div class="w-[5px] h-[65px] lg:h-[100%] bg-[#D8D8D8] mx-auto"></div>
          </div>
          <div class="ml-5 md:ml-10 mt-[15px] md:mt-[0px]">
            <h2
              class="text-[#0D47A1] font-medium not-italic md:text-[30px] lg:text-[40px] lg:leading-[80px]"
            >
              Seguimiento y guía
            </h2>
            <p
              class="text-start not-italic font-normal text-[10px] md:text-[15px] lg:text-[22px] lg:leading-[30px]"
            >
              Eche un vistazo a la ruta que ya esta tomando el conductor para
              llegar a usted. Rastree su ubicación exacta y guielo si es
              necesario.
            </p>
          </div>
        </div>

        <div class="flex">
          <div>
            <div
              class="w-[50px] h-[50px] md:w-[70px] md:h-[70px] rounded-[50%] bg-[#EAEAEA] border-2 border-[#D8D8D8] text-[#FFFFFF] text-center text-[45px] font-medium md:font-semibold md:leading-[60px]"
            >
              4
            </div>
          </div>
          <div class="ml-5 md:ml-10 mt-[15px] md:mt-[0px]">
            <h2
              class="text-[#0D47A1] font-medium not-italic md:text-[30px] lg:text-[40px] lg:leading-[80px]"
            >
              Súbete y viaja
            </h2>
            <p
              class="text-start not-italic font-normal text-[10px] md:text-[15px] lg:text-[22px] lg:leading-[30px]"
            >
              Una vez que el conductor te alcance, solo súbete y disfruta del
              viaje. La aplicación calculara la tarifa y le dará una factura al
              final del viaje.
            </p>
          </div>
        </div>
      </div>
      <HowFunctionMobile class="flex items-center" />
    </div>
  </div>
</template>
