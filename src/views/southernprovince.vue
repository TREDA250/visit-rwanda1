<script setup>
import { useI18n } from '../i18n.js'
const { t } = useI18n()

const destinations = [
  {
    nameKey: 'regions.southern.place1',
    descriptionKey: 'regions.southern.place1Desc',
    image: 'src/assets/nyungwe.png',
  },
  {
    nameKey: 'regions.southern.place2',
    descriptionKey: 'regions.southern.place2Desc',
    image: 'src/assets/ingoro.jpg',
  },
  {
    nameKey: 'regions.southern.place3',
    descriptionKey: 'regions.southern.place3Desc',
    image: 'src/assets/Ethnographic.jpg',
  },
]
</script>

<template>
  <div class="bg-gray-100 min-h-screen py-10">
    <div class="container mx-auto px-6">
      <h1 class="text-5xl font-bold text-center text-blue-700 mb-8">{{ t('regions.southern.title') }}</h1>

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