<template>
  <section class="py-14 md:py-24 bg-gray-50 text-zinc-900">
    <div class="container px-8 mx-auto">
      <div class="flex flex-col max-w-xl justify-center items-center text-center mx-auto">
        <h2 class="text-3xl font-bold md:text-[45px] mb-4">Como funciona?</h2>
        <p class="text-lg opacity-80">
          A participação é simples e rápida! Veja o passo a passo para se inscrever e jogar.
        </p>
      </div>

      <div class="grid grid-cols-4 gap-6 gap-y-16 mt-16 lg:gap-y-0 lg:mt-12">
        <!-- card start -->
        <div class="col-span-4 sm:col-span-2 lg:col-span-1 h-52 w-72">
          <div
            class="bg-white shadow-xl rounded-xl flex flex-col justify-center items-center text-center pb-10 px-6 h-full"
          >
            <div
              class="w-20 h-20 rounded-full bg-red-500 bg-opacity-90 flex items-center justify-center -translate-y-10"
            >
              <h1 class="font-medium text-[40px] text-white">1</h1>
            </div>
            <h2 class="text-2xl font-medium">Escolha o jogo</h2>
            <div class="font-medium">
              <Icon icon="bx:bxs-joystick" class="w-20 h-20" />
              <span class="text-xs">League of Legends, TFT, Valorant...</span>
            </div>
          </div>
        </div>
        <!-- card end -->
        <!-- card start -->
        <div class="col-span-4 sm:col-span-2 lg:col-span-1 h-52 w-72">
          <div
            class="bg-white shadow-xl rounded-xl flex flex-col justify-center items-center text-center pb-10 px-6 h-full"
          >
            <div
              class="w-20 h-20 rounded-full bg-yellow-500 bg-opacity-90 flex items-center justify-center -translate-y-10"
            >
              <h1 class="font-medium text-[40px] text-white">2</h1>
            </div>
            <h2 class="text-2xl font-medium">Monte sua equipe</h2>
            <div class="font-medium">
              <Icon icon="fluent:people-team-32-filled" class="w-20 h-20" />
              <span class="text-xs">Reúna seus amigos e colegas</span>
            </div>
          </div>
        </div>
        <!-- card end -->
        <!-- card start -->
        <div class="col-span-4 sm:col-span-2 lg:col-span-1 h-52 w-72">
          <div
            class="bg-white shadow-xl rounded-xl flex flex-col justify-center items-center text-center pb-10 px-6 h-full"
          >
            <div
              class="w-20 h-20 rounded-full bg-green-500 bg-opacity-90 flex items-center justify-center -translate-y-10"
            >
              <h1 class="font-medium text-[40px] text-white">3</h1>
            </div>
            <h2 class="text-2xl font-medium">Faça a inscrição</h2>
            <div class="font-medium">
              <Icon icon="lets-icons:ticket-use-fill" class="w-20 h-20" />
              <span class="text-xs">Veja como se inscrever nos card abaixo</span>
            </div>
          </div>
        </div>
        <!-- card end -->
        <!-- card start -->
        <div class="col-span-4 sm:col-span-2 lg:col-span-1 h-52 w-72">
          <div
            class="bg-blue-500 shadow-xl rounded-xl flex flex-col justify-center items-center text-center pb-10 px-6 h-full"
          >
            <div
              class="w-20 h-20 rounded-full bg-white flex items-center justify-center -translate-y-10"
            >
              <h1 class="font-medium text-[40px] text-blue-400">4</h1>
            </div>
            <h2 class="text-white text-2xl font-medium grow">Partir pro abraço!</h2>
            <p class="text-white leading-relaxed grow drop-shadow-lg shadow-black">
              Depois de se inscrever, é só jogar e se divertir!
            </p>
          </div>
        </div>
        <!-- card end -->
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
import { Icon } from '@iconify/vue'
</script>
