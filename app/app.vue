<script setup>
const config = useRuntimeConfig()
const baseURL = config.app.baseURL

const images = [
  'IMG_20240217_133633.jpg',
  'IMG_20240217_190752.jpg',
  'IMG_20240217_190858.jpg',
  'IMG_20240217_192629.jpg',
  'IMG_20240218_174710.jpg',
  'IMG_20240218_203131.jpg',
  'IMG_20240218_204236.jpg',
  'IMG_20240218_204906.jpg',
  'IMG_20240218_211904.jpg',
  'IMG_20240221_225312.jpg',
  'IMG_20240331_003152_810.jpg',
  'IMG-20240528-WA0058.jpg',
  'WhatsApp Image 2026-05-06 at 13.36.10 (1).jpeg',
  'WhatsApp Image 2026-05-06 at 13.36.10.jpeg',
  'WhatsApp Image 2026-05-06 at 13.36.11 (1).jpeg',
  'WhatsApp Image 2026-05-06 at 13.36.11.jpeg'
]
</script>

<template>
  <div class="min-h-screen bg-slate-50 text-slate-900 font-sans selection:bg-blue-100">
    <NuxtRouteAnnouncer />
    
    <main class="max-w-4xl mx-auto px-6 py-16 md:py-24">
      <!-- Hero Section -->
      <header class="mb-16">
        <h1 class="text-4xl md:text-5xl font-light tracking-tight mb-4">Surfboard for Sale</h1>
        <div class="flex flex-wrap gap-4 items-baseline">
          <p class="text-2xl font-medium text-blue-600">Rp 5.000.000</p>
          <p class="text-slate-500 italic">All included</p>
        </div>
      </header>

      <!-- Specifications Grid -->
      <section class="grid md:grid-cols-2 gap-12 mb-20">
        <div>
          <h2 class="text-xs uppercase tracking-widest font-semibold text-slate-400 mb-6">Specifications</h2>
          <ul class="space-y-4">
            <li class="flex justify-between border-b border-slate-200 pb-2">
              <span class="text-slate-500">Dimensions</span>
              <span class="font-medium">6'2" × 21" × 2 5/8"</span>
            </li>
            <li class="flex justify-between border-b border-slate-200 pb-2">
              <span class="text-slate-500">Volume</span>
              <span class="font-medium">36 Liters</span>
            </li>
            <li class="flex justify-between border-b border-slate-200 pb-2">
              <span class="text-slate-500">Fin System</span>
              <span class="font-medium">Thruster (Futures)</span>
            </li>
          </ul>
        </div>

        <div>
          <h2 class="text-xs uppercase tracking-widest font-semibold text-slate-400 mb-6">Included Accessories</h2>
          <ul class="space-y-4 text-slate-700">
            <li class="flex items-center gap-2">
              <span class="w-1.5 h-1.5 rounded-full bg-blue-500"></span>
              3x Futures Honey Comb Fins
            </li>
            <li class="flex items-center gap-2">
              <span class="w-1.5 h-1.5 rounded-full bg-blue-500"></span>
              Dakine Leash
            </li>
          </ul>
        </div>
      </section>

      <!-- About the Board -->
      <section class="mb-20">
        <h2 class="text-xs uppercase tracking-widest font-semibold text-slate-400 mb-6">About the Board</h2>
        <div class="prose prose-slate max-w-none text-slate-700 leading-relaxed space-y-4">
          <p>
            Designed with generous volume, this board is <strong>exceptionally easy to paddle</strong> and catches waves effortlessly, even in smaller or weaker conditions. It is the ideal companion for anyone looking for a chill ride or intermediate surfers aiming to progress.
          </p>
          <p>
            While it excels in everyday surf, it remains remarkably stable and reliable when the swell picks up, holding its line comfortably in waves up to <strong>8ft (2.5m)</strong>.
          </p>
        </div>
      </section>

      <!-- Condition & Location -->
      <section class="mb-20">
        <h2 class="text-xs uppercase tracking-widest font-semibold text-slate-400 mb-6">Condition & Location</h2>
        <div class="prose prose-slate max-w-none text-slate-700 leading-relaxed space-y-4">
          <p>
            Purchased brand new in 2023, this board has been ridden for approximately <strong>30 sessions</strong>. Since late 2023, it has been stored in a clean, dry environment.
          </p>
          <p>
            Overall, the board is in good condition. It shows typical light pressure marks on the deck from normal use and one small compression mark on the top rail.
          </p>
          <div class="mt-8 p-6 bg-slate-100 rounded-lg border border-slate-200">
            <p class="text-sm font-medium mb-1">Viewing Location:</p>
            <p class="text-slate-600">Visible in <strong>Jimbaran</strong>. Exact address available upon request via the contact links below.</p>
          </div>
        </div>
      </section>

      <!-- Gallery -->
      <section>
        <h2 class="text-xs uppercase tracking-widest font-semibold text-slate-400 mb-8">Gallery</h2>
        <div class="columns-1 sm:columns-2 lg:columns-3 gap-4 space-y-4">
          <div v-for="img in images" :key="img" class="break-inside-avoid">
            <img 
              :src="`${baseURL}${img}`" 
              class="w-full rounded-lg shadow-sm hover:shadow-md transition-shadow duration-300 border border-slate-200"
              alt="Surfboard detail"
            />
          </div>
        </div>
      </section>

      <!-- Contact / Footer -->
      <footer class="mt-32 pt-12 border-t border-slate-200 text-center">
        <p class="text-slate-500 text-sm mb-6">Interested? Contact for more details or to arrange a viewing.</p>
        
        <div class="flex flex-col sm:flex-row justify-center items-center gap-6 mb-12">
          <a 
            href="https://wa.me/33658215300" 
            target="_blank"
            class="flex items-center gap-2 text-slate-700 hover:text-green-600 transition-colors"
          >
            <span class="font-medium">WhatsApp:</span> +33 6 58 21 53 00
          </a>
          <a 
            href="https://www.instagram.com/starfox_adventure/" 
            target="_blank"
            class="flex items-center gap-2 text-slate-700 hover:text-pink-600 transition-colors"
          >
            <span class="font-medium">Instagram:</span> @starfox_adventure
          </a>
        </div>

        <p class="text-slate-300 text-xs">2026 &copy; Surfboard Sale</p>
      </footer>
    </main>
  </div>
</template>

<style>
body {
  @apply bg-slate-50;
}
</style>
