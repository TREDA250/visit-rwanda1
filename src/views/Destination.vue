<script setup>
import { useI18n } from '../i18n.js'
const { t } = useI18n()
</script>

<template>
  <div class="bg-gray-50 min-h-screen">
    <section class="relative h-[80vh]">
      <img
        src="https://images.unsplash.com/photo-1501785888041-af3ef285b470"
        alt="Rwanda"
        class="w-full h-full object-cover"
      />
      <div class="absolute inset-0 bg-black/60 flex items-center justify-center">
        <div class="text-center text-white px-6">
          <h1 class="text-6xl md:text-7xl font-bold mb-6">{{ t('destination.heroTitle') }}</h1>
          <p class="text-xl max-w-3xl mx-auto">{{ t('destination.heroText') }}</p>
        </div>
      </div>
    </section>

    <section class="py-16">
      <div class="container mx-auto px-6">
        <h2 class="text-5xl font-bold text-center text-green-700 mb-4">{{ t('destination.attractionsTitle') }}</h2>
        <p class="text-center text-gray-600 max-w-3xl mx-auto mb-12">{{ t('destination.attractionsText') }}</p>
        <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
          <div class="bg-white rounded-2xl overflow-hidden shadow-lg hover:shadow-2xl hover:-translate-y-2 transition">
            <img src="https://images.unsplash.com/photo-1500530855697-b586d89ba3ee" class="h-64 w-full object-cover" />
            <div class="p-6">
              <span class="text-green-600 font-semibold">{{ t('nav.northernProvince') }}</span>
              <h3 class="text-2xl font-bold mt-2">{{ t('destination.volcanoesTitle') }}</h3>
              <p class="text-gray-600 mt-3">{{ t('destination.volcanoesText') }}</p>
            </div>
          </div>
          <div class="bg-white rounded-2xl overflow-hidden shadow-lg hover:shadow-2xl hover:-translate-y-2 transition">
            <img src="https://images.unsplash.com/photo-1549366021-9f761d450615" class="h-64 w-full object-cover" />
            <div class="p-6">
              <span class="text-yellow-600 font-semibold">{{ t('nav.easternProvince') }}</span>
              <h3 class="text-2xl font-bold mt-2">{{ t('destination.akageraTitle') }}</h3>
              <p class="text-gray-600 mt-3">{{ t('destination.akageraText') }}</p>
            </div>
          </div>
          <div class="bg-white rounded-2xl overflow-hidden shadow-lg hover:shadow-2xl hover:-translate-y-2 transition">
            <img src="https://images.unsplash.com/photo-1441974231531-c6227db76b6e" class="h-64 w-full object-cover" />
            <div class="p-6">
              <span class="text-blue-600 font-semibold">{{ t('nav.southernProvince') }}</span>
              <h3 class="text-2xl font-bold mt-2">{{ t('regions.southern.place1') }}</h3>
              <p class="text-gray-600 mt-3">{{ t('regions.southern.place1Desc') }}</p>
            </div>
          </div>
          <div class="bg-white rounded-2xl overflow-hidden shadow-lg hover:shadow-2xl hover:-translate-y-2 transition">
            <img src="https://images.unsplash.com/photo-1507525428034-b723cf961d3e" class="h-64 w-full object-cover" />
            <div class="p-6">
              <span class="text-cyan-600 font-semibold">{{ t('nav.westernProvince') }}</span>
              <h3 class="text-2xl font-bold mt-2">{{ t('regions.western.place1') }}</h3>
              <p class="text-gray-600 mt-3">{{ t('regions.western.place1Desc') }}</p>
            </div>
          </div>
          <div class="bg-white rounded-2xl overflow-hidden shadow-lg hover:shadow-2xl hover:-translate-y-2 transition">
            <img src="https://images.unsplash.com/photo-1511818966892-d7d671e672a2" class="h-64 w-full object-cover" />
            <div class="p-6">
              <span class="text-purple-600 font-semibold">{{ t('nav.kigaliCity') }}</span>
              <h3 class="text-2xl font-bold mt-2">{{ t('regions.kigali.place1') }}</h3>
              <p class="text-gray-600 mt-3">{{ t('regions.kigali.place1Desc') }}</p>
            </div>
          </div>
          <div class="bg-white rounded-2xl overflow-hidden shadow-lg hover:shadow-2xl hover:-translate-y-2 transition">
            <img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb" class="h-64 w-full object-cover" />
            <div class="p-6">
              <span class="text-green-600 font-semibold">{{ t('nav.northernProvince') }}</span>
              <h3 class="text-2xl font-bold mt-2">{{ t('regions.northern.place3') }}</h3>
              <p class="text-gray-600 mt-3">{{ t('regions.northern.place3Desc') }}</p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="bg-green-700 text-white py-16">
      <div class="container mx-auto px-6">
        <div class="grid md:grid-cols-4 gap-8 text-center">
          <div>
            <h3 class="text-5xl font-bold">5</h3>
            <p class="mt-2">{{ t('gallery.stat1') }}</p>
          </div>
          <div>
            <h3 class="text-5xl font-bold">3</h3>
            <p class="mt-2">{{ t('gallery.stat2') }}</p>
          </div>
          <div>
            <h3 class="text-5xl font-bold">100+</h3>
            <p class="mt-2">{{ t('gallery.stat3') }}</p>
          </div>
          <div>
            <h3 class="text-5xl font-bold">1M+</h3>
            <p class="mt-2">{{ t('gallery.stat4') }}</p>
          </div>
        </div>
      </div>
    </section>

    <section class="py-20 bg-white text-center">
      <h2 class="text-5xl font-bold text-gray-800 mb-6">{{ t('destination.ctaTitle') }}</h2>
      <p class="text-gray-600 text-lg mb-8">{{ t('destination.ctaText') }}</p>
      <button class="bg-green-700 hover:bg-green-800 text-white px-10 py-4 rounded-full font-semibold transition">
        {{ t('destination.ctaButton') }}
      </button>
    </section>
  </div>
</template>