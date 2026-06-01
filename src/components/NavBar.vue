<script setup>
import { computed } from 'vue'
import { useI18n } from '../i18n.js'

const { t, locale, setLocale } = useI18n()
const languages = computed(() => [
  { code: 'en', label: t('language.english') },
  { code: 'fr', label: t('language.french') },
  { code: 'rw', label: t('language.kinyarwanda') },
])
</script>

<template>
  <nav class="bg-green-800 text-white px-8 py-4 flex flex-col md:flex-row items-center justify-between shadow-lg gap-4">
    <div class="flex items-center gap-4">
      <img src="/public/image.png" alt="logo" class="rounded-full w-10 h-10" />
      <ul class="flex gap-6 text-sm font-medium">
        <li>
          <router-link to="/" class="hover:text-yellow-300">{{ t('nav.home') }}</router-link>
        </li>
        <li>
          <router-link to="/about" class="hover:text-yellow-300">{{ t('nav.about') }}</router-link>
        </li>
        <li>
          <router-link to="/services" class="hover:text-yellow-300">{{ t('nav.services') }}</router-link>
        </li>
        <li class="group relative">
          <button type="button" class="hover:text-yellow-300 inline-flex items-center gap-1">{{ t('nav.gallery') }}<span>▼</span></button>
          <ul class="invisible group-hover:visible opacity-0 group-hover:opacity-100 absolute bg-white text-green-900 rounded shadow w-48 z-50 pt-2" style="top: 100%">
            <li>
              <router-link to="/photos" class="block px-4 py-2 hover:bg-green-200">{{ t('nav.photos') }}</router-link>
            </li>
            <li>
              <router-link to="/videos" class="block px-4 py-2 hover:bg-green-200">{{ t('nav.videos') }}</router-link>
            </li>
          </ul>
        </li>
        <li class="group relative">
          <button type="button" class="hover:text-yellow-300 inline-flex items-center gap-1">{{ t('nav.destinations') }}<span>▼</span></button>
          <ul class="invisible group-hover:visible opacity-0 group-hover:opacity-100 absolute bg-white text-green-900 rounded shadow w-56 z-50 pt-2" style="top: 100%">
            <li>
              <router-link to="/northernprovince" class="block px-4 py-2 hover:bg-green-200">{{ t('nav.northernProvince') }}</router-link>
            </li>
            <li>
              <router-link to="/southernprovince" class="block px-4 py-2 hover:bg-green-200">{{ t('nav.southernProvince') }}</router-link>
            </li>
            <li>
              <router-link to="/kigalicity" class="block px-4 py-2 hover:bg-green-200">{{ t('nav.kigaliCity') }}</router-link>
            </li>
            <li>
              <router-link to="/easternprovince" class="block px-4 py-2 hover:bg-green-200">{{ t('nav.easternProvince') }}</router-link>
            </li>
            <li>
              <router-link to="/westernprovince" class="block px-4 py-2 hover:bg-green-200">{{ t('nav.westernProvince') }}</router-link>
            </li>
          </ul>
        </li>
        <li>
          <router-link to="/contact" class="hover:text-yellow-300">{{ t('nav.contact') }}</router-link>
        </li>
      </ul>
    </div>
    <div class="flex items-center gap-3">
      <label class="text-sm">{{ t('language.switcher') }}:</label>
      <select
        v-model="locale"
        @change="setLocale(locale)"
        class="rounded-lg bg-white text-green-900 px-3 py-1"
      >
        <option v-for="lang in languages" :key="lang.code" :value="lang.code">
          {{ lang.label }}
        </option>
      </select>
    </div>
  </nav>
</template>