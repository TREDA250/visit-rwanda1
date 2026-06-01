<script setup>
import { useI18n } from '../i18n.js'
const { t } = useI18n()

const destinations = [
  {
    nameKey: 'regions.northern.place1',
    descriptionKey: 'regions.northern.place1Desc',
    image: 'https://images.unsplash.com/photo-1500530855697-b586d89ba3ee',
  },
  {
    nameKey: 'regions.northern.place2',
    descriptionKey: 'regions.northern.place2Desc',
    image: 'https://images.unsplash.com/photo-1511497584788-876760111969',
  },
  {
    nameKey: 'regions.northern.place3',
    descriptionKey: 'regions.northern.place3Desc',
    image: 'https://images.unsplash.com/photo-1506744038136-46273834b3fb',
  },
]
</script>

<template>
  <div class="bg-gray-100 min-h-screen py-10">
    <div class="container mx-auto px-6">
      <h1 class="text-5xl font-bold text-center text-green-700 mb-8">{{ t('regions.northern.title') }}</h1>
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