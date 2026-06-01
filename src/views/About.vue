<script setup>
import { useI18n } from '../i18n.js'
const { t } = useI18n()
</script>

<template>
  <div class="bg-gray-100 min-h-screen">
    <section
      class="h-96 bg-cover bg-center flex items-center justify-center"
      style="background-image: url('https://images.unsplash.com/photo-1526778548025-fa2f459cd5ce?q=80&w=1600&auto=format&fit=crop');"
    ></section>

    <section class="py-16 px-8 max-w-6xl mx-auto">
      <div class="grid grid-cols-1 md:grid-cols-2 gap-10 items-center">
        <div>
          <img
            src="https://images.unsplash.com/photo-1516426122078-c23e76319801?q=80&w=1200&auto=format&fit=crop"
            class="rounded-2xl shadow-xl"
          />
        </div>

        <div>
          <h2 class="text-4xl font-bold text-green-700 mb-6">{{ t('about.title') }}</h2>
          <p class="text-gray-700 text-lg mb-4">{{ t('about.paragraph1') }}</p>
          <p class="text-gray-700 text-lg mb-4">{{ t('about.paragraph2') }}</p>
          <p class="text-gray-700 text-lg mb-4">{{ t('about.paragraph3') }}</p>
          <button class="bg-green-700 hover:bg-green-800 text-white px-6 py-3 rounded-lg mt-4">{{ t('about.button') }}</button>
        </div>
      </div>
    </section>

    <section class="bg-white py-16 px-8">
      <h2 class="text-4xl font-bold text-center text-green-700 mb-12">{{ t('about.whyTitle') }}</h2>
      <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
        <div class="bg-gray-100 p-8 rounded-2xl shadow-md text-center">
          <h3 class="text-2xl font-bold mb-4">{{ t('home.features.clean') }}</h3>
          <p>{{ t('home.featureText.clean') }}</p>
        </div>
        <div class="bg-gray-100 p-8 rounded-2xl shadow-md text-center">
          <h3 class="text-2xl font-bold mb-4">{{ t('home.features.wildlife') }}</h3>
          <p>{{ t('home.featureText.wildlife') }}</p>
        </div>
        <div class="bg-gray-100 p-8 rounded-2xl shadow-md text-center">
          <h3 class="text-2xl font-bold mb-4">{{ t('home.features.culture') }}</h3>
          <p>{{ t('home.featureText.culture') }}</p>
        </div>
      </div>
    </section>
  </div>
</template>