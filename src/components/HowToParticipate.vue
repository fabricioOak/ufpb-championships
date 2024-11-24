<template>
  <section class="py-14 mb-20 md:py-24 bg-gray-50 text-zinc-900">
    <div class="container px-4 mx-auto">
      <div class="flex flex-col max-w-xl justify-center items-center text-center mx-auto">
        <h2 class="text-3xl font-bold md:text-[45px] mb-4">Como funciona?</h2>
        <p class="text-lg opacity-80">
          A participação é simples e rápida! Veja o passo a passo para se inscrever e jogar.
        </p>
      </div>

      <div class="grid grid-cols-4 gap-6 gap-y-16 mt-16 lg:gap-y-0 lg:mt-12">
        <!-- card start -->
        <div class="col-span-4 sm:col-span-2 lg:col-span-1 h-60 w-80">
          <div
            class="bg-white shadow-xl rounded-xl flex flex-col justify-center items-center text-center pb-10 px-6 h-full"
          >
            <div
              class="w-20 h-20 rounded-full bg-purple-600 bg-opacity-90 flex items-center justify-center -translate-y-10"
            >
              <h1 class="font-medium text-[40px] text-white">1</h1>
            </div>
            <h2 class="text-2xl font-medium">Escolha o jogo</h2>
            <div class="font-medium">
              <v-icon name="io-game-controller" class="w-20 h-20" />
            </div>
          </div>
        </div>
        <!-- card end -->
        <!-- card start -->
        <div class="col-span-4 sm:col-span-2 lg:col-span-1 h-60 w-80">
          <div
            class="bg-white shadow-xl rounded-xl flex flex-col justify-center items-center text-center pb-10 px-6 h-full"
          >
            <div
              class="w-20 h-20 rounded-full bg-purple-600 bg-opacity-90 flex items-center justify-center -translate-y-10"
            >
              <h1 class="font-medium text-[40px] text-white">2</h1>
            </div>
            <h2 class="text-2xl font-medium">Monte sua equipe</h2>
            <div class="font-medium"><v-icon name="ri-team-fill" class="w-20 h-20" /></div>
          </div>
        </div>
        <!-- card end -->
        <!-- card start -->
        <div class="col-span-4 sm:col-span-2 lg:col-span-1 h-60 w-80">
          <div
            class="bg-white shadow-xl rounded-xl flex flex-col justify-center items-center text-center pb-10 px-6 h-full"
          >
            <div
              class="w-20 h-20 rounded-full bg-purple-600 bg-opacity-90 flex items-center justify-center -translate-y-10"
            >
              <h1 class="font-medium text-[40px] text-white">3</h1>
            </div>
            <h2 class="text-2xl font-medium">Faça a inscrição</h2>
            <v-icon name="co-notes" class="w-20 h-20" />
            <div class="font-medium"></div>
          </div>
        </div>
        <!-- card end -->
        <!-- card start -->
        <div class="col-span-4 sm:col-span-2 lg:col-span-1 h-60 w-80">
          <div
            class="bg-purple-600 shadow-xl rounded-xl flex flex-col justify-center items-center text-center pb-10 px-6 h-full"
          >
            <div
              class="w-20 h-20 rounded-full bg-white flex items-center justify-center -translate-y-10"
            >
              <h1 class="font-medium text-[40px]">4</h1>
            </div>
            <h2 class="text-white text-2xl font-medium grow">Partir pro abraço!</h2>
            <p class="text-white leading-relaxed grow opacity-75">
              Depois de se inscrever, é só jogar e se divertir!
            </p>
          </div>
        </div>
        <!-- card end -->
      </div>
    </div>
  </section>
</template>
