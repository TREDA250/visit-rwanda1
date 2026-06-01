<script setup>
import { useI18n } from '../i18n.js'
const { t } = useI18n()

const destinations = [
  {
    nameKey: 'regions.western.place1',
    descriptionKey: 'regions.western.place1Desc',
    image: 'https://images.unsplash.com/photo-1501785888041-af3ef285b470',
  },
  {
    nameKey: 'regions.western.place2',
    descriptionKey: 'regions.western.place2Desc',
    image: 'https://images.unsplash.com/photo-1470770903676-69b98201ea1c',
  },
  {
    nameKey: 'regions.western.place3',
    descriptionKey: 'regions.western.place3Desc',
    image: 'https://images.unsplash.com/photo-1500534623283-312aade485b7',
  },
]
</script>

<template>
  <div class="bg-gray-100 min-h-screen py-10">
    <div class="container mx-auto px-6">
      <h1 class="text-5xl font-bold text-center text-cyan-700 mb-8">{{ t('regions.western.title') }}</h1>

      <div class="grid md:grid-cols-3 gap-8">
        <div
          v-for="place in destinations"
          :key="place.nameKey"
          class="bg-white rounded-xl overflow-hidden shadow-lg hover:scale-105 transition"
        >
          <img :src="place.image" class="h-60 w-full object-cover" />
          <div class="p-5">
            <h2 class="text-2xl font-bold mb-2">{{ t(place.nameKey) }}</h2>
            <p class="text-gray-600">{{ t(place.descriptionKey) }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>