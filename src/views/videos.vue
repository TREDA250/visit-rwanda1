<script setup>
import { useI18n } from '../i18n.js'
const { t } = useI18n()
</script>

<template>
  <div class="bg-gray-100 min-h-screen">
    <section class="bg-green-700 text-white py-16">
      <div class="container mx-auto text-center px-6">
        <h1 class="text-5xl font-bold mb-4">{{ t('videos.heroTitle') }}</h1>
        <p class="text-xl">{{ t('videos.heroText') }}</p>
      </div>
    </section>

    <section class="container mx-auto px-6 py-16">
      <div class="grid md:grid-cols-2 gap-10">
        <div class="bg-white rounded-2xl shadow-lg overflow-hidden">
          <iframe
            class="w-full h-80"
            src="https://www.youtube.com/embed/aqz-KE-bpKQ"
            title="Visit Rwanda"
            allowfullscreen
          ></iframe>
          <div class="p-6">
            <h2 class="text-2xl font-bold text-green-700">{{ t('videos.video1Title') }}</h2>
            <p class="text-gray-600 mt-2">{{ t('videos.video1Text') }}</p>
          </div>
        </div>
        <div class="bg-white rounded-2xl shadow-lg overflow-hidden">
          <iframe
            class="w-full h-80"
            src="https://www.youtube.com/embed/aqz-KE-bpKQ"
            title="Mountain Gorillas"
            allowfullscreen
          ></iframe>
          <div class="p-6">
            <h2 class="text-2xl font-bold text-green-700">{{ t('videos.video2Title') }}</h2>
            <p class="text-gray-600 mt-2">{{ t('videos.video2Text') }}</p>
          </div>
        </div>
        <div class="bg-white rounded-2xl shadow-lg overflow-hidden">
          <iframe
            class="w-full h-80"
            src="https://www.youtube.com/embed/aqz-KE-bpKQ"
            title="Akagera National Park"
            allowfullscreen
          ></iframe>
          <div class="p-6">
            <h2 class="text-2xl font-bold text-green-700">{{ t('videos.video3Title') }}</h2>
            <p class="text-gray-600 mt-2">{{ t('videos.video3Text') }}</p>
          </div>
        </div>
        <div class="bg-white rounded-2xl shadow-lg overflow-hidden">
          <iframe
            class="w-full h-80"
            src="https://www.youtube.com/embed/aqz-KE-bpKQ"
            title="Lake Kivu"
            allowfullscreen
          ></iframe>
          <div class="p-6">
            <h2 class="text-2xl font-bold text-green-700">{{ t('videos.video4Title') }}</h2>
            <p class="text-gray-600 mt-2">{{ t('videos.video4Text') }}</p>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>