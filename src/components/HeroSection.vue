<template>
  <header
    class="bg-cover bg-right bg-no-repeat text-white relative flex justify-center items-center py-40 md:py-48 z-[1]"
  >
    <div
      class="absolute top-0 left-0 right-0 bottom-0 -z-[1]"
      style="background: linear-gradient(130deg, rgba(255, 185, 25, 0.35), rgba(0, 0, 0, 0.831))"
    ></div>
    <div class="container px-4">
      <div class="grid grid-cols-12">
        <div class="col-span-12 md:col-span-9 lg:col-span-7 xl:col-span-6">
          <h2 class="text-[32px] leading-snug md:text-8xl font-bold tracking-wider mb-6">
            Una-se a Gloriosa Evolução!
          </h2>
          <p class="text-lg leading-relaxed mb-12 md:mr-32 lg:mr-52">
            Bem-vindo ao Campeonato de eSports da UFPB 2025! Esta é a oportunidade perfeita para os
            gamers da nossa universidade mostrarem suas habilidades. <br />
            Forme sua equipe, desafie os adversários e alcance o topo nos jogos eletrônicos.
          </p>
          <div class="md:mr-40 lg:mr-72">
            <button
              class="py-4 px-8 text-bold bg-yellow-600 ring-2 ring-amber-500 hover:-translate-y-1 transition text-slate-50 font-bold hover:bg-opacity-80 rounded-full w-full"
            >
              Saiba Mais Sobre o Evento
            </button>
          </div>
        </div>
      </div>
      <div class="absolute bottom-4 md:bottom-12 left-1/2 w-full -translate-x-1/2">
        <div class="flex flex-wrap items-center justify-center mt-12"></div>
      </div>
    </div>
  </header>
</template>

<style scoped>
header {
  background-image: url('../assets/images/hero-2.jpg');
  @apply bg-cover bg-no-repeat text-white relative flex justify-center items-center py-40 md:py-48 z-[1] bg-center sm:bg-right;
}
</style>
