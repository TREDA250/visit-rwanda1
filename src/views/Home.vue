<script setup>
import { useI18n } from '../i18n.js'
const { t } = useI18n()
</script>

<template>
  <div class="bg-gray-100">

    <!-- Hero Section -->
    <section
      class="h-screen bg-cover bg-center flex items-center justify-center"
      style="background-image: url('https://images.unsplash.com/photo-1516426122078-c23e76319801?q=80&w=1600&auto=format&fit=crop');"
    >
      <div class="bg-green bg-opacity-60 p-10 rounded-xl text-center text-white">
        <h1 class="text-5xl font-bold mb-4">{{ t('home.heroTitle') }}</h1>
        <p class="text-xl mb-6">{{ t('home.heroText') }}</p>
      </div>
    </section>

    <!-- Attractions -->
    <section class="py-16 px-6">
      <h2 class="text-4xl font-bold text-center text-green-700 mb-10">{{ t('home.heroTitle') }}</h2>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
        <div class="bg-white rounded-2xl shadow-lg overflow-hidden">
          <img
            src="https://images.unsplash.com/photo-1547471080-7cc2caa01a7e?q=80&w=1200&auto=format&fit=crop"
            class="w-full h-60 object-cover"
          />
          <div class="p-5">
            <h3 class="text-2xl font-bold text-green-700 mb-3">{{ t('home.card1Title') }}</h3>
            <p class="text-gray-600">{{ t('home.card1Text') }}</p>
          </div>
        </div>
        <div class="bg-white rounded-2xl shadow-lg overflow-hidden">
          <img
            src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?q=80&w=1200&auto=format&fit=crop"
            class="w-full h-60 object-cover"
          />
          <div class="p-5">
            <h3 class="text-2xl font-bold text-green-700 mb-3">{{ t('home.card2Title') }}</h3>
            <p class="text-gray-600">{{ t('home.card2Text') }}</p>
          </div>
        </div>
        <div class="bg-white rounded-2xl shadow-lg overflow-hidden">
          <img
            src="https://images.unsplash.com/photo-1516026672322-bc52d61a55d5?q=80&w=1200&auto=format&fit=crop"
            class="w-full h-60 object-cover"
          />
          <div class="p-5">
            <h3 class="text-2xl font-bold text-green-700 mb-3">{{ t('home.card3Title') }}</h3>
            <p class="text-gray-600">{{ t('home.card3Text') }}</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Welcome -->
    <section class="bg-green-700 text-white py-16 text-center px-6">
      <h2 class="text-4xl font-bold mb-4">{{ t('home.welcomeTitle') }}</h2>
      <p class="max-w-3xl mx-auto text-lg">{{ t('home.welcomeText') }}</p>
    </section>
  </div>
</template>