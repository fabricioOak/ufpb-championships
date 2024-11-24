<template>
  <div class="z-10 py-6 bg-white text-zinc-900 relative">
    <nav>
      <div class="container px-4">
        <div class="flex justify-between items-center">
          <!-- Logo -->
          <div>
            <img class="max-h-8" src="../assets/images/ufpb_esports.png" alt="" srcset="" />
          </div>

          <!-- Botão do Menu (Hambúrguer) -->
          <button
            class="block md:hidden cursor-pointer h-10 z-20"
            type="button"
            @click="toggleMenu"
          >
            <div class="h-0.5 w-7 bg-black -translate-y-2"></div>
            <div class="h-0.5 w-7 bg-black"></div>
            <div class="h-0.5 w-7 bg-black translate-y-2"></div>
          </button>

          <!-- Menu de Navegação -->
          <ul
            :class="[
              'flex flex-col md:flex-row justify-center items-center text-3xl gap-6 md:text-base md:gap-2 absolute md:relative top-0 md:top-auto md:left-auto w-screen md:w-auto h-screen md:h-auto bg-white md:bg-transparent transition-all',
              isMenuOpen ? 'left-0' : 'left-full max-xl:hidden',
            ]"
          >
            <li>
              <a class="px-4 opacity-100" href="#">Home</a>
            </li>
            <li>
              <a class="px-4 opacity-50 hover:opacity-100" href="#">Services</a>
            </li>
            <li>
              <a class="px-4 opacity-50 hover:opacity-100" href="#">Why us?</a>
            </li>
            <li>
              <a class="px-4 opacity-50 hover:opacity-100" href="#">How It Works</a>
            </li>
            <li>
              <a class="px-4 opacity-50 hover:opacity-100" href="#">Features</a>
            </li>
            <li>
              <a class="px-4 opacity-50 hover:opacity-100" href="#">Testimonials</a>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

// Estado para controlar o menu
const isMenuOpen = ref(false)

// Função para alternar o estado do menu
const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value
}
</script>

<style scoped>
/* Transições suaves para o menu */
ul {
  transition: left 0.3s ease-in-out;
}
</style>
