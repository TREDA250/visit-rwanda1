<template>
  <nav class="bg-green-800 text-white px-8 py-4 flex items-center justify-between shadow-lg">
    <img src="/public/image.png" alt="logo" class="rounded-full w-10 h-10">

    <ul class="flex gap-8 text-sm font-medium">
      <li>
        <router-link to="/" class="hover:text-yellow-300 cursor-pointer">Home</router-link>
      </li>
      <li>
        <router-link to="/about" class="hover:text-yellow-300 cursor-pointer">About Us</router-link>
      </li>
      <li>
        <router-link to="/services" class="hover:text-yellow-300 cursor-pointer">Services</router-link>
      </li>
      <li class="group relative">
        <button type="button" class="hover:text-yellow-300 cursor-pointer inline-flex items-center gap-1">Gallery<span>▼</span></button>
        <ul class="invisible group-hover:visible opacity-0 group-hover:opacity-100 absolute bg-white text-green-900 rounded shadow w-48 z-50 pt-2" style="top: 100%">
          <li>
            <router-link to="/photos" class="block px-4 py-2 hover:bg-green-200 text-green-900">Photos</router-link>
          </li>
          <li>
            <router-link to="/videos" class="block px-4 py-2 hover:bg-green-200 text-green-900">Videos</router-link>
          </li>
        </ul>
      </li>
      <li class="group relative">
        <button type="button" class="hover:text-yellow-300 cursor-pointer inline-flex items-center gap-1">Destinations<span>▼</span></button>
        <ul class="invisible group-hover:visible opacity-0 group-hover:opacity-100 absolute bg-white text-green-900 rounded shadow w-56 z-50 pt-2" style="top: 100%">
          <li>
            <router-link to="/northernprovince" class="block px-4 py-2 text-green-900 hover:bg-green-200">Northern Province</router-link>
          </li>
          <li>
            <router-link to="/southernprovince" class="block px-4 py-2 text-green-900 hover:bg-green-200">Southern Province</router-link>
          </li>
          <li>
            <router-link to="/kigalicity" class="block px-4 py-2 text-green-900 hover:bg-green-200">Kigali City</router-link>
          </li>
          <li>
            <router-link to="/easternprovince" class="block px-4 py-2 text-green-900 hover:bg-green-200">Eastern Province</router-link>
          </li>
          <li>
            <router-link to="/westernprovince" class="block px-4 py-2 text-green-900 hover:bg-green-200">Western Province</router-link>
          </li>
        </ul>
      </li>
      <li>
        <router-link to="/contact" class="hover:text-yellow-300 cursor-pointer">Contact</router-link>
      </li>
    </ul>
  </nav>
</template>