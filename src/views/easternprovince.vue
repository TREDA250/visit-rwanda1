<script setup>
import { useI18n } from '../i18n.js'
const { t } = useI18n()

const destinations = [
  {
    nameKey: 'regions.eastern.place1',
    descriptionKey: 'regions.eastern.place1Desc',
    image: 'https://images.unsplash.com/photo-1549366021-9f761d450615',
  },
  {
    nameKey: 'regions.eastern.place2',
    descriptionKey: 'regions.eastern.place2Desc',
    image: 'https://images.unsplash.com/photo-1507525428034-b723cf961d3e',
  },
  {
    nameKey: 'regions.eastern.place3',
    descriptionKey: 'regions.eastern.place3Desc',
    image: 'https://images.unsplash.com/photo-1470770841072-f978cf4d019e',
  },
]
</script>

<template>
  <div class="bg-gray-100 min-h-screen py-10">
    <div class="container mx-auto px-6">
      <h1 class="text-5xl font-bold text-center text-yellow-600 mb-8">{{ t('regions.eastern.title') }}</h1>

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