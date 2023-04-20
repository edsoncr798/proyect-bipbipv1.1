<script lang="ts" setup>
import { defineComponent, ref } from 'vue';

const isSelected = ref(false);

const isSelectedClicks = async() => {
    // isSelected.value = !isSelected.value;
    // console.log(isSelected.value)
}
</script>


<template>
  <div class="max-w-[1065px]">
    <div
      class="mx-auto border-[7px] border-black w-[283px] h-[516.15px] rounded-[20px]"
    >
      <div
        class="rounded-bl-[10px] rounded-br-[10px] mx-auto bg-black w-[70%] h-[20px]"
      ></div>
      <div class="md:blur-[5px] w-full mt-[40px] px-[10px]">
        <div class="flex" @click="isSelectedClicks">
          <div>
            <div
              :class="{'selected-step': isSelected}"
              class="w-[50px] h-[50px]  rounded-[50%] bg-[#0D47A1]  text-[#FFFFFF] text-center text-[20px] font-medium leading-[45px]"
            >
              1
            </div>
            <div 
              :class="{'selected-step': isSelected}"
              class="w-[5px] h-[50%] bg-[#0D47A1] mx-auto">
            </div>
          </div>
          <div class="ml-5 mt-[15px]">
            <h2
              class="text-[#0D47A1] font-medium not-italic "
            >
              Toca para reservar
            </h2>
            <p
              class="text-start not-italic font-normal text-[10px] "
            >
              Solo levanta tu teléfono y colócalo donde quieras ir. La
              aplicación te convertirá en un conductor en poco tiempo.
            </p>
          </div>
        </div>

        <div class="flex" @click="isSelectedClicks">
          <div>
            <div
            :class="{'selected-step': isSelected}"
              class="w-[50px] h-[50px] rounded-[50%] bg-[#EAEAEA] border-2 border-[#D8D8D8] text-[#FFFFFF] text-center text-[20px] font-medium leading-[45px]"
            >
              2
            </div>
            <div
              :class="{'selected-step': isSelected}" 
              class="w-[5px] h-[60%] bg-[#D8D8D8] mx-auto"></div>
          </div>
          <div class="ml-5 mt-[15px]">
            <h2
              class="text-[#0D47A1] font-medium not-italic "
            >
              Detalles de conductor
            </h2>
            <p
              class="text-start not-italic font-normal text-[10px] "
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
              class="w-[50px] h-[50px] rounded-[50%] bg-[#EAEAEA] border-2 border-[#D8D8D8] text-[#FFFFFF] text-center text-[20px] font-medium leading-[45px]"
            >
              3
            </div>
            <div class="w-[5px] h-[50%] bg-[#D8D8D8] mx-auto"></div>
          </div>
          <div class="ml-5 mt-[15px]">
            <h2
              class="text-[#0D47A1] font-medium not-italic "
            >
              Seguimiento y guía
            </h2>
            <p
              class="text-start not-italic font-normal text-[10px] "
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
              class="w-[50px] h-[50px] rounded-[50%] bg-[#EAEAEA] border-2 border-[#D8D8D8] text-[#FFFFFF] text-center text-[20px] font-medium leading-[45px]"
            >
              4
            </div>
          </div>
          <div class="ml-5 mt-[15px]">
            <h2
              class="text-[#0D47A1] font-medium not-italic "
            >
              Súbete y viaja
            </h2>
            <p
              class="text-start not-italic font-normal text-[10px] "
            >
              Una vez que el conductor te alcance, solo súbete y disfruta del
              viaje. La aplicación calculara la tarifa y le dará una factura al
              final del viaje.
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>


<style scope>
.selected-step{
  background:#0D47A1;
  border: none;
}
</style>
