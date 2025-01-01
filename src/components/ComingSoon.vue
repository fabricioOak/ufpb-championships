<template>
  <section
    class="py-36 md:py-72 text-white bg-cover bg-center bg-no-repeat relative overflow-hidden z-[1] waiting"
  >
    <div class="absolute top-0 left-0 right-0 bottom-0 bg-black bg-opacity-55 -z-[1]"></div>
    <div class="container px-4">
      <div class="grid grid-cols-12">
        <div class="col-span-12 md:col-span-6 lg:col-span-5 xl:col-span-4">
          <div class="text-center md:text-start">
            <h2 class="text-[32px] md:text-[65px] leading-none font-bold mb-4">
              <em>Se liga na data!</em>
            </h2>
            <p class="text-lg opacity-80 ml-2 flex">
              <em>Vocês podem acompanhar o evento ao vivo na <em>Twitch</em></em>
              <a class="ml-2" target="_blank" href="http:////www.twitch.tv/gamersufpb">
                <Icon icon="simple-icons:twitch" class="h-8 w-8 text-purple-500" />
              </a>
            </p>

            <!-- <form
              class="bg-white bg-opacity-10 rounded-[50px] overflow-hidden text-white flex items-center mt-6 md:mr-12"
            >
              <input
                name="email"
                class="bg-transparent py-4 px-5 placeholder:text-lg placeholder:text-opacity-60 focus:outline-none grow"
                type="email"
                placeholder="Enter email"
                required
              />
              <button class="text-xl font-semibold duration-500 hover:text-blue-600 mr-7">
                <i class="fas fa-paper-plane"></i>
              </button>
            </form> -->
          </div>
        </div>
      </div>
    </div>

    <!-- countdown -->
    <div
      class="absolute bottom-12 left-1/2 -translate-x-1/2 min-w-[100px] md:top-1/2 md:bottom-[15%] md:left-[85%] md:translate-x-0 md:-translate-y-1/2 lg:left-[70%] flex md:flex-col items-center"
    >
      <div class="flex flex-col text-center p-4">
        <span class="text-4xl leading-none font-bold">{{ days }}</span>
        <span class="text-base opacity-50">Dias</span>
      </div>

      <div class="flex flex-col text-center p-4">
        <span class="text-4xl leading-none font-bold">{{ hours }}</span>
        <span class="text-base opacity-50">Horas</span>
      </div>
      <div class="flex flex-col text-center p-4">
        <span class="text-4xl leading-none font-bold">{{ minutes }}</span>
        <span class="text-base opacity-50">Minutos</span>
      </div>
      <div class="flex flex-col text-center p-4">
        <span class="text-4xl leading-none font-bold">{{ seconds }}</span>
        <span class="text-base opacity-50">Segundos</span>
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
import { ref, onMounted, onBeforeUnmount } from 'vue'
import { Icon } from '@iconify/vue'

const days = ref('00')
const hours = ref('00')
const minutes = ref('00')
const seconds = ref('00')
const targetDate = new Date('2025-01-11T00:00:00')
let timer: number

const updateCountdown = () => {
  const now = new Date()
  const distance = targetDate.getTime() - now.getTime()

  if (distance <= 0) {
    clearInterval(timer)
    days.value = '00'
    hours.value = '00'
    minutes.value = '00'
    seconds.value = '00'
    return
  }

  days.value = String(Math.floor(distance / (1000 * 60 * 60 * 24))).padStart(2, '0')
  hours.value = String(Math.floor((distance / (1000 * 60 * 60)) % 24)).padStart(2, '0')
  minutes.value = String(Math.floor((distance / (1000 * 60)) % 60)).padStart(2, '0')
  seconds.value = String(Math.floor((distance / 1000) % 60)).padStart(2, '0')
}

const startCountdown = () => {
  updateCountdown()
  timer = setInterval(updateCountdown, 1000)
}

onMounted(() => {
  startCountdown()
})

onBeforeUnmount(() => {
  clearInterval(timer)
})
</script>

<style scoped>
.waiting {
  background-image: url('../assets/images/waiting.jpg');
}
</style>
