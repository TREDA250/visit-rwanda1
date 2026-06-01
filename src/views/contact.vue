<script setup>
import { useI18n } from '../i18n.js'
const { t } = useI18n()
</script>

<template>
  <div class="bg-gray-100 min-h-screen">
    <section class="relative h-[60vh]">
      <img
        src="https://images.unsplash.com/photo-1501785888041-af3ef285b470"
        alt="Contact Rwanda"
        class="w-full h-full object-cover"
      />

      <div class="absolute inset-0 bg-black/60 flex items-center justify-center">
        <div class="text-center text-white px-6">
          <h1 class="text-6xl md:text-7xl font-bold mb-4">{{ t('contact.heroTitle') }}</h1>
          <p class="text-xl">{{ t('contact.heroText') }}</p>
        </div>
      </div>
    </section>

    <section class="container mx-auto px-6 py-20">
      <div class="grid lg:grid-cols-2 gap-12">
        <div class="bg-white p-8 rounded-2xl shadow-lg">
          <h2 class="text-4xl font-bold text-green-700 mb-8">{{ t('contact.getInTouch') }}</h2>
          <div class="space-y-6">
            <div class="flex items-center gap-4">
              <span class="text-3xl">📍</span>
              <div>
                <h3 class="font-bold text-lg">{{ t('contact.addressTitle') }}</h3>
                <p class="text-gray-600">{{ t('contact.addressText') }}</p>
              </div>
            </div>
            <div class="flex items-center gap-4">
              <span class="text-3xl">📞</span>
              <div>
                <h3 class="font-bold text-lg">{{ t('contact.phoneTitle') }}</h3>
                <p class="text-gray-600">{{ t('contact.phoneText1') }}</p>
                <p class="text-gray-600">{{ t('contact.phoneText2') }}</p>
              </div>
            </div>
            <div class="flex items-center gap-4">
              <span class="text-3xl">📧</span>
              <div>
                <h3 class="font-bold text-lg">{{ t('contact.emailTitle') }}</h3>
                <p class="text-gray-600">{{ t('contact.emailText1') }}</p>
                <p class="text-gray-600">{{ t('contact.emailText2') }}</p>
              </div>
            </div>
            <div class="flex items-center gap-4">
              <span class="text-3xl">🕒</span>
              <div>
                <h3 class="font-bold text-lg">{{ t('contact.hoursTitle') }}</h3>
                <p class="text-gray-600">{{ t('contact.hoursText') }}</p>
              </div>
            </div>
          </div>
          <div class="mt-10">
            <h3 class="text-2xl font-bold mb-4">{{ t('contact.followUs') }}</h3>
            <div class="flex gap-4">
              <a href="#" class="bg-blue-600 text-white px-5 py-3 rounded-lg hover:bg-blue-700">Facebook</a>
              <a href="#" class="bg-pink-600 text-white px-5 py-3 rounded-lg hover:bg-pink-700">Instagram</a>
              <a href="#" class="bg-black text-white px-5 py-3 rounded-lg hover:bg-gray-800">X</a>
            </div>
          </div>
        </div>

        <div class="bg-white p-8 rounded-2xl shadow-lg">
          <h2 class="text-4xl font-bold text-green-700 mb-8">{{ t('contact.sendMessage') }}</h2>
          <form class="space-y-6">
            <div>
              <label class="block mb-2 font-semibold">{{ t('contact.fullName') }}</label>
              <input
                type="text"
                :placeholder="t('contact.placeholderName')"
                class="w-full border border-gray-300 rounded-lg p-4 focus:outline-none focus:ring-2 focus:ring-green-600"
              />
            </div>
            <div>
              <label class="block mb-2 font-semibold">{{ t('contact.emailAddress') }}</label>
              <input
                type="email"
                :placeholder="t('contact.placeholderEmail')"
                class="w-full border border-gray-300 rounded-lg p-4 focus:outline-none focus:ring-2 focus:ring-green-600"
              />
            </div>
            <div>
              <label class="block mb-2 font-semibold">{{ t('contact.subject') }}</label>
              <input
                type="text"
                :placeholder="t('contact.placeholderSubject')"
                class="w-full border border-gray-300 rounded-lg p-4 focus:outline-none focus:ring-2 focus:ring-green-600"
              />
            </div>
            <div>
              <label class="block mb-2 font-semibold">{{ t('contact.message') }}</label>
              <textarea
                rows="6"
                :placeholder="t('contact.placeholderMessage')"
                class="w-full border border-gray-300 rounded-lg p-4 focus:outline-none focus:ring-2 focus:ring-green-600"
              ></textarea>
            </div>
            <button
              type="submit"
              class="bg-green-700 hover:bg-green-800 text-white px-8 py-4 rounded-lg font-semibold transition"
            >
              {{ t('contact.submitButton') }}
            </button>
          </form>
        </div>
      </div>
    </section>

    <section class="pb-20 px-6">
      <div class="container mx-auto">
        <div class="bg-white rounded-2xl shadow-lg overflow-hidden">
          <iframe
            src="https://maps.google.com/maps?q=Kigali%20Rwanda&t=&z=13&ie=UTF8&iwloc=&output=embed"
            allowfullscreen=""
            loading="lazy"
          ></iframe>
        </div>
      </div>
    </section>
  </div>
</template>