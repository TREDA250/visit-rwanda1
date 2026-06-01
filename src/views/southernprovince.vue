<template>
  <div class="bg-gray-100 min-h-screen py-10">
    <div class="container mx-auto px-6">
      <h1 class="text-5xl font-bold text-center text-blue-700 mb-8">
        Southern Province
      </h1>

      <div class="grid md:grid-cols-3 gap-8">
        <div
          v-for="place in destinations"
          :key="place.name"
          class="bg-white rounded-xl overflow-hidden shadow-lg hover:scale-105 transition"
        >
          <img :src="place.image" class="h-60 w-full object-cover" />
          <div class="p-5">
            <h2 class="text-2xl font-bold mb-2">{{ place.name }}</h2>
            <p class="text-gray-600">{{ place.description }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const destinations = [
  {
    name: "Nyungwe Forest",
    image: "src/assets/nyungwe.png",
    description: "Ancient rainforest famous for canopy walks and chimpanzees."
  },
  {
    name: "King's Palace Museum",
    image: "src/assets/ingoro.jpg",
    description: "Traditional royal residence preserving Rwanda's heritage."
  },
  {
    name: "Ethnographic Museum",
    image: "src/assets/Ethnographic.jpg",
    description: "One of Africa's finest cultural museums."
  }
]
</script>