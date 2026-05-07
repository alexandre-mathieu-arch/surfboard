<script setup>
const config = useRuntimeConfig()
const baseURL = config.app.baseURL

// Main hero image
const heroImage = 'IMG-20240528-WA0058.jpg'

const images = [
  { name: 'IMG_20240217_133633.jpg', current: false },
  { name: 'IMG_20240217_190752.jpg', current: false },
  { name: 'IMG_20240217_190858.jpg', current: false },
  { name: 'IMG_20240217_192629.jpg', current: false },
  { name: 'IMG_20240218_170032.jpg', current: false },
  { name: 'IMG_20240218_174710.jpg', current: false },
  { name: 'IMG_20240218_203131.jpg', current: false },
  { name: 'IMG_20240218_204236.jpg', current: false },
  { name: 'IMG_20240218_204906.jpg', current: false },
  { name: 'IMG_20240218_211904.jpg', current: false },
  { name: 'IMG_20240221_225312.jpg', current: false },
  { name: 'IMG_20240331_003152_810.jpg', current: false },
  { name: 'WhatsApp Image 2026-05-06 at 13.36.10 (1).jpeg', current: true },
  { name: 'WhatsApp Image 2026-05-06 at 13.36.10.jpeg', current: true },
  { name: 'WhatsApp Image 2026-05-06 at 13.36.11 (1).jpeg', current: true },
  { name: 'WhatsApp Image 2026-05-06 at 13.36.11.jpeg', current: true }
]
</script>

<template>
  <div class="min-h-screen bg-white text-slate-900 font-sans selection:bg-slate-100">
    <NuxtRouteAnnouncer />
    
    <main class="max-w-4xl mx-auto px-6 py-16 md:py-24">
      <!-- Header Section -->
      <header class="mb-16">
        <div class="flex flex-col md:flex-row md:items-baseline justify-between gap-2 mb-4">
          <h1 class="text-3xl md:text-5xl font-light tracking-tight text-slate-900">
            6'2" Allround for sale:
          </h1>
          <p class="text-xl font-medium text-slate-500 uppercase tracking-widest text-sm md:text-base">South Bali • Jimbaran</p>
        </div>
        
        <p class="text-xl text-slate-600 mb-4 font-light italic">
          Surfboard + complete accessories ready for the water
        </p>

        <div class="mb-8 flex items-center gap-4">
          <span class="inline-block px-3 py-1 bg-slate-100 text-slate-600 text-xs font-semibold uppercase tracking-widest rounded">
            Second Hand • Excellent Condition
          </span>
          <a href="#contact" class="text-xs font-bold uppercase tracking-widest border-b-2 border-slate-900 pb-0.5 hover:text-slate-500 hover:border-slate-500 transition-all">
            Get in touch
          </a>
        </div>

        <div class="prose prose-slate mb-8">
          <p class="text-slate-600 italic">
            "Selling my board because I am moving."
          </p>
        </div>

        <!-- Hero Image -->
        <div class="mb-16 overflow-hidden rounded-lg border border-slate-100">
          <img 
            :src="`${baseURL}${heroImage}`" 
            class="w-full h-auto object-cover"
            alt="Surfboard Hero"
          />
          <div class="bg-slate-900 text-white text-[10px] py-2 px-3 uppercase tracking-[0.1em] font-semibold text-center">
            Current Condition
          </div>
        </div>

        <div class="flex flex-wrap gap-4 items-baseline justify-between border-b border-slate-100 pb-8">
          <div class="flex flex-col">
            <p class="text-slate-400 text-sm uppercase tracking-widest font-semibold mb-1">All included</p>
            <p class="text-4xl font-medium text-slate-900">Rp 4.950.000</p>
          </div>
          <p class="text-slate-400 italic">Complete pack</p>
        </div>
      </header>

      <!-- Specifications Grid -->
      <section class="grid md:grid-cols-2 gap-16 mb-24">
        <div>
          <h2 class="text-xs uppercase tracking-widest font-semibold text-slate-400 mb-8">Specifications</h2>
          <ul class="space-y-4">
            <li class="flex justify-between border-b border-slate-100 pb-2">
              <span class="text-slate-500">Dimensions</span>
              <span class="font-medium">6'2" × 21" × 2 5/8"</span>
            </li>
            <li class="flex justify-between border-b border-slate-100 pb-2">
              <span class="text-slate-500">Volume</span>
              <span class="font-medium">36 Liters</span>
            </li>
            <li class="flex justify-between border-b border-slate-100 pb-2">
              <span class="text-slate-500">Material</span>
              <span class="font-medium">PU (polyurethane)</span>
            </li>
            <li class="flex justify-between border-b border-slate-100 pb-2">
              <span class="text-slate-500">Fin System</span>
              <span class="font-medium">Thruster (Futures)</span>
            </li>
          </ul>
        </div>

        <div>
          <h2 class="text-xs uppercase tracking-widest font-semibold text-slate-400 mb-8">Included Pack</h2>
          <ul class="space-y-4 text-slate-700">
            <li class="flex flex-col border-b border-slate-100 pb-2">
              <div class="flex items-center gap-2">
                <span class="w-1 h-1 bg-slate-400 rounded-full"></span>
                <span class="font-medium">Surfboard Colorsurf All-round 6'2"</span>
              </div>
              <span class="text-xs text-slate-400 ml-3">Shaped by Chris Cutch (Channel Islands). New value: Rp 7,000,000</span>
            </li>
            <li class="flex flex-col border-b border-slate-100 pb-2">
              <div class="flex items-center gap-2">
                <span class="w-1 h-1 bg-slate-400 rounded-full"></span>
                <span class="font-medium">Futures Fins Signature</span>
              </div>
              <span class="text-xs text-slate-400 ml-3">New value: Rp 1,850,000</span>
            </li>
            <li class="flex flex-col border-b border-slate-100 pb-2">
              <div class="flex items-center gap-2">
                <span class="w-1 h-1 bg-slate-400 rounded-full"></span>
                <span class="font-medium">Leash Dakine Kainui Plus</span>
              </div>
              <span class="text-xs text-slate-400 ml-3">New value: Rp 599,000</span>
            </li>
          </ul>
        </div>
      </section>

      <!-- About the Board -->
      <section class="mb-24">
        <h2 class="text-xs uppercase tracking-widest font-semibold text-slate-400 mb-8">Performance & Origin</h2>
        <div class="prose prose-slate max-w-none text-slate-600 leading-relaxed space-y-6">
          <p>
            This is a <strong>COLORSURF</strong> board shaped by <strong>Chris Cutch</strong>. Chris is a renowned local shaper who also shapes for <strong>Channel Islands Surfboards</strong>. This board features the same technical and performance characteristics as an <strong>Al Merrick</strong> board.
          </p>
          <p>
            Designed with generous volume, this board is exceptionally easy to paddle and catches waves effortlessly, even in smaller conditions. Ideal for chill sessions or intermediate surfers aiming to progress.
          </p>
          <p>
            Remarkably stable and reliable when the swell picks up, holding its line comfortably in waves up to 8ft (2.5m).
          </p>
        </div>
      </section>

      <!-- Condition & Location -->
      <section class="mb-24">
        <h2 class="text-xs uppercase tracking-widest font-semibold text-slate-400 mb-8">Status & Location</h2>
        <div class="grid md:grid-cols-2 gap-8 bg-slate-50 p-8 rounded-lg border border-slate-100">
          <div>
            <p class="text-sm font-medium text-slate-900 mb-2">History</p>
            <p class="text-slate-600 text-sm leading-relaxed">
              Purchased new in 2024. Ridden for ~30 sessions. Meticulously stored in clean/dry conditions since late 2024. Light deck pressure marks, one minor rail compression.
            </p>
          </div>
          <div class="md:border-l md:border-slate-200 md:pl-8">
            <p class="text-sm font-medium text-slate-900 mb-2">Viewing</p>
            <p class="text-slate-600 text-sm leading-relaxed">
              Visible in <strong>Jimbaran, South Bali</strong>. Exact address provided upon request.
            </p>
          </div>
        </div>
      </section>

      <!-- Gallery -->
      <section>
        <h2 class="text-xs uppercase tracking-widest font-semibold text-slate-400 mb-12">Detailed Gallery</h2>
        <div class="columns-1 sm:columns-2 lg:columns-3 gap-4 space-y-4">
          <div v-for="img in images" :key="img.name" class="break-inside-avoid relative group">
            <div class="rounded overflow-hidden border border-slate-100 shadow-sm">
              <img 
                :src="`${baseURL}${img.name}`" 
                class="w-full h-auto object-cover"
                alt="Surfboard detail"
              />
              <div v-if="img.current" class="bg-slate-900 text-white text-[10px] py-1.5 px-3 uppercase tracking-[0.1em] font-semibold text-center">
                Current Condition
              </div>
            </div>
          </div>
        </div>
      </section>

      <!-- Contact / Footer -->
      <footer id="contact" class="mt-32 pt-16 border-t border-slate-100 text-center">
        <p class="text-slate-400 text-sm mb-10 italic">Contact for details or viewing</p>
        
        <div class="flex flex-col sm:flex-row justify-center items-center gap-8 mb-20">
          <a 
            href="https://wa.me/33658215300" 
            target="_blank"
            class="text-slate-900 font-medium border-b border-slate-900 hover:text-slate-500 hover:border-slate-500 transition-all"
          >
            WhatsApp
          </a>
          <a 
            href="https://www.instagram.com/starfox_adventure/" 
            target="_blank"
            class="text-slate-900 font-medium border-b border-slate-900 hover:text-slate-500 hover:border-slate-500 transition-all"
          >
            Instagram
          </a>
          <a 
            href="https://www.facebook.com/share/1ELBbu4pBJ/" 
            target="_blank"
            class="text-slate-900 font-medium border-b border-slate-900 hover:text-slate-500 hover:border-slate-500 transition-all"
          >
            Facebook
          </a>
        </div>

        <p class="text-slate-300 text-[10px] tracking-[0.2em] uppercase">2026 &copy; Bali Surfboard Sale</p>
      </footer>
    </main>
  </div>
</template>

<style>
body {
  @apply bg-white;
}
</style>
