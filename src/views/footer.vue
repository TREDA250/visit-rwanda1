<script setup>
import { useI18n } from '../i18n.js'

const { t } = useI18n()
</script>

<template>
  <footer class="bg-green-800 text-white px-8 py-10 mt-10">
    <div class="flex flex-wrap justify-between gap-8">
      <div>
        <h3 class="text-yellow-300 font-bold text-lg mb-3">{{ t('footer.title') }}</h3>
        <p class="text-sm text-green-200">{{ t('footer.subtitle') }}</p>
      </div>

      <div>
        <h3 class="text-yellow-300 font-bold text-lg mb-3">{{ t('footer.quickLinks') }}</h3>
        <ul class="space-y-2 text-sm">
          <li><RouterLink to="/" class="text-green-200 hover:text-yellow-300">{{ t('nav.home') }}</RouterLink></li>
          <li><RouterLink to="/about" class="text-green-200 hover:text-yellow-300">{{ t('nav.about') }}</RouterLink></li>
          <li><RouterLink to="/contact" class="text-green-200 hover:text-yellow-300">{{ t('nav.contact') }}</RouterLink></li>
          <li><RouterLink to="/services" class="text-green-200 hover:text-yellow-300">{{ t('nav.services') }}</RouterLink></li>
        </ul>
      </div>

      <div>
        <h3 class="text-yellow-300 font-bold text-lg mb-3">{{ t('footer.destinations') }}</h3>
        <ul class="text-sm space-y-2">
          <li><RouterLink to="/kigalicity" class="text-green-200 hover:text-yellow-300">{{ t('nav.kigaliCity') }}</RouterLink></li>
          <li><RouterLink to="/northernprovince" class="text-green-200 hover:text-yellow-300">{{ t('nav.northernProvince') }}</RouterLink></li>
          <li><RouterLink to="/southernprovince" class="text-green-200 hover:text-yellow-300">{{ t('nav.southernProvince') }}</RouterLink></li>
          <li><RouterLink to="/easternprovince" class="text-green-200 hover:text-yellow-300">{{ t('nav.easternProvince') }}</RouterLink></li>
          <li><RouterLink to="/westernprovince" class="text-green-200 hover:text-yellow-300">{{ t('nav.westernProvince') }}</RouterLink></li>
        </ul>
      </div>

      <div>
        <h3 class="text-yellow-300 font-bold text-lg mb-3">{{ t('footer.contact') }}</h3>
        <ul class="text-sm space-y-2">
          <li class="text-green-300">{{ t('contact.addressText') }}</li>
          <li class="text-green-300">{{ t('contact.phoneTitle') }}: {{ t('contact.phoneText1') }}</li>
          <li class="text-green-300">{{ t('contact.emailTitle') }}: {{ t('contact.emailText1') }}</li>
        </ul>
      </div>
    </div>
    <div class="border-t border-green-600 mt-8 pt-4 text-sm">
      <p class="text-center">{{ t('footer.copyright') }}</p>
    </div>
  </footer>
</template>