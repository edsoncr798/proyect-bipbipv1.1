<script lang="ts" setup>
</script>
<template>
    <header class='w-full absolute md:p-6 z-10 h-16 '>
        <div class="justify-between min-w-[835px] container max-w-[1450px] items-center w-4/5 flex  h-full mx-auto">
            <div class="flex w-[450px] justify-between items-center">
                <div class="h-10 w-32">
                    <img class="" src="../../../images/logo_whitebg.png" alt="">
                </div>
                <div class="">
                    <button class="truncate">Sobre Nosotros</button>
                    <button class="truncate">Contáctenos</button>
                </div>
            </div>
            <div class="w-[280px] flex justify-between">
                <button class="bg-white truncate font-medium">Iniciar Sesión</button>
                <button class="bg-white truncate font-medium">Registrarse</button>
            </div>
        </div>
    </header>
</template>

<style>
header{
    background: rgba(255, 255, 255, 0.4);
    box-shadow: 4px 7px 15px rgba(0, 0, 0, 0.08), inset -5px 5px 12px rgba(255, 255, 255, 0.05);
    backdrop-filter: blur(15px);
}
</style>