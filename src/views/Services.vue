<script setup>
import { useI18n } from '../i18n.js'
const { t } = useI18n()
</script>

<template>
  <div class="bg-gray-50 min-h-screen">
    <section class="relative h-[70vh]">
      <img
        src="https://images.unsplash.com/photo-1506744038136-46273834b3fb"
        alt="Rwanda Tourism"
        class="w-full h-full object-cover"
      />

      <div class="absolute inset-0 bg-black/60 flex items-center justify-center">
        <div class="text-center text-white px-6">
          <h1 class="text-5xl md:text-7xl font-bold mb-4">{{ t('services.heroTitle') }}</h1>
          <p class="text-lg md:text-2xl max-w-3xl mx-auto">{{ t('services.heroText') }}</p>
        </div>
      </div>
    </section>

    <section class="py-16">
      <div class="container mx-auto px-6">
        <h2 class="text-4xl font-bold text-center text-green-700 mb-4">{{ t('services.title') }}</h2>
        <p class="text-center text-gray-600 max-w-3xl mx-auto mb-12">{{ t('services.subtitle') }}</p>

        <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
          <div class="bg-white rounded-2xl overflow-hidden shadow-lg hover:shadow-2xl hover:-translate-y-2 transition duration-300">
            <img
              src="https://images.unsplash.com/photo-1516939884455-1445c8652f83"
              class="h-56 w-full object-cover"
            />
            <div class="p-6">
              <h3 class="text-2xl font-bold text-green-700 mb-3">{{ t('services.service1') }}</h3>
              <p class="text-gray-600">{{ t('services.service1Text') }}</p>
            </div>
          </div>
          <div class="bg-white rounded-2xl overflow-hidden shadow-lg hover:shadow-2xl hover:-translate-y-2 transition duration-300">
            <img
              src="https://images.unsplash.com/photo-1516426122078-c23e76319801"
              class="h-56 w-full object-cover"
            />
            <div class="p-6">
              <h3 class="text-2xl font-bold text-green-700 mb-3">{{ t('services.service2') }}</h3>
              <p class="text-gray-600">{{ t('services.service2Text') }}</p>
            </div>
          </div>
          <div class="bg-white rounded-2xl overflow-hidden shadow-lg hover:shadow-2xl hover:-translate-y-2 transition duration-300">
            <img
              src="https://images.unsplash.com/photo-1507525428034-b723cf961d3e"
              class="h-56 w-full object-cover"
            />
            <div class="p-6">
              <h3 class="text-2xl font-bold text-green-700 mb-3">{{ t('services.service3') }}</h3>
              <p class="text-gray-600">{{ t('services.service3Text') }}</p>
            </div>
          </div>
          <div class="bg-white rounded-2xl overflow-hidden shadow-lg hover:shadow-2xl hover:-translate-y-2 transition duration-300">
            <img
              src="https://images.unsplash.com/photo-1441974231531-c6227db76b6e"
              class="h-56 w-full object-cover"
            />
            <div class="p-6">
              <h3 class="text-2xl font-bold text-green-700 mb-3">{{ t('services.service4') }}</h3>
              <p class="text-gray-600">{{ t('services.service4Text') }}</p>
            </div>
          </div>
          <div class="bg-white rounded-2xl overflow-hidden shadow-lg hover:shadow-2xl hover:-translate-y-2 transition duration-300">
            <img
              src="https://images.unsplash.com/photo-1511818966892-d7d671e672a2"
              class="h-56 w-full object-cover"
            />
            <div class="p-6">
              <h3 class="text-2xl font-bold text-green-700 mb-3">{{ t('services.service5') }}</h3>
              <p class="text-gray-600">{{ t('services.service5Text') }}</p>
            </div>
          </div>
          <div class="bg-white rounded-2xl overflow-hidden shadow-lg hover:shadow-2xl hover:-translate-y-2 transition duration-300">
            <img
              src="https://images.unsplash.com/photo-1521295121783-8a321d551ad2"
              class="h-56 w-full object-cover"
            />
            <div class="p-6">
              <h3 class="text-2xl font-bold text-green-700 mb-3">{{ t('services.service6') }}</h3>
              <p class="text-gray-600">{{ t('services.service6Text') }}</p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="bg-green-700 text-white py-16">
      <div class="container mx-auto px-6">
        <h2 class="text-4xl font-bold text-center mb-12">{{ t('services.whyTitle') }}</h2>

        <div class="grid md:grid-cols-4 gap-8 text-center">
          <div>
            <div class="text-5xl mb-4">🌍</div>
            <h3 class="text-xl font-bold">{{ t('services.benefit1') }}</h3>
            <p class="mt-2">{{ t('services.benefit1Text') }}</p>
          </div>
          <div>
            <div class="text-5xl mb-4">🦍</div>
            <h3 class="text-xl font-bold">{{ t('services.benefit2') }}</h3>
            <p class="mt-2">{{ t('services.benefit2Text') }}</p>
          </div>
          <div>
            <div class="text-5xl mb-4">🏨</div>
            <h3 class="text-xl font-bold">{{ t('services.benefit3') }}</h3>
            <p class="mt-2">{{ t('services.benefit3Text') }}</p>
          </div>
          <div>
            <div class="text-5xl mb-4">⭐</div>
            <h3 class="text-xl font-bold">{{ t('services.benefit4') }}</h3>
            <p class="mt-2">{{ t('services.benefit4Text') }}</p>
          </div>
        </div>
      </div>
    </section>

    <section class="py-20 bg-white">
      <div class="container mx-auto px-6 text-center">
        <h2 class="text-5xl font-bold text-gray-800 mb-4">{{ t('destination.ctaTitle') }}</h2>
        <p class="text-gray-600 text-lg mb-8">{{ t('destination.ctaText') }}</p>
        <button class="bg-green-700 hover:bg-green-800 text-white px-10 py-4 rounded-full text-lg font-semibold transition">
          {{ t('destination.ctaButton') }}
        </button>
      </div>
    </section>
  </div>
</template>