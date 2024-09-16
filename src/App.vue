<template>
  <!-- <h1 class="text-3xl font-bold underline">Hello world!</h1> -->
  <!-- Opcion #1 lo tradicional dentro de vue -->
  <!-- <PrincipalPagina />
  <ContactoPagina />
  <PreciosPagina />
  <FeaturesPagina /> -->
  <div class="flex flex-col h-screen">
    <!-- Header -->
    <header class="flex items-center h-14 px-4 border-b border-gray-300 sm:h-16 md:px-6 lg:px-8">
      <div>
        <a class="flex items-center gap-2 font-semibold" href="#">
          <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="40" height="40" />
        </a>
      </div>
      <nav class="ml-auto space-x-4 flex items-center h-10 sm:space-x-6">
        <RouterLink to="/">Principal</RouterLink><br />
        <RouterLink to="/FeaturesPagina">Features</RouterLink><br />
        <RouterLink to="/ContactoPagina">Contacto</RouterLink><br />
        <RouterLink to="/PreciosPagina">Precios</RouterLink>
      </nav>
    </header>
    <!-- Fin Header -->

    <!-- <nav> -->
    <!-- Opcion #2 con lo tradicional al html -->
    <!-- <a href="#/">Principal</a><br />
    <a href="#/">Contacto</a><br />
    <a href="#/">Precios</a><br />
    <a href="#/">Features</a><br />

      <RouterLink to="/">Principal</RouterLink><br />
      <RouterLink to="/FeaturesPagina">Features</RouterLink><br />
      <RouterLink to="/ContactoPagina">Contacto</RouterLink><br />
      <RouterLink to="/PreciosPagina">Precios</RouterLink> -->
    <!-- </nav> -->

    <!-- Main -->
    <main class="flex-1 flex items-center justify-center py-6">
      <div class="text-center">
        <RouterView />
      </div>
    </main>
    <!-- Fin Main -->

    <!-- Footer -->
    <footer class="flex items-center h-14 px-4 border-t border-gray-300 sm:h-16 md:px-6 lg:px-8">
      <p class="flex-1 text-sm text-gray-500 text-center">
        © {{ currentYear }} Acme Corporation. Derechos reservados
      </p>
    </footer>
    <!-- Fin Footer -->
  </div>
</template>

<script lang="ts" setup>
// Opcion #1 lo tradicional
// import PrincipalPagina from './modules/landing/pages/PrincipalPagina.vue'
// import ContactoPagina from './modules/landing/pages/ContactoPagina.vue'
// import PreciosPagina from './modules/landing/pages/PreciosPagina.vue'
// import FeaturesPagina from './modules/landing/pages/FeaturesPagina.vue'

import { ref, onMounted } from 'vue'

// Definimos una variable reactiva tipada como número
const currentYear = ref<number>(0)

// Asignamos el año actual directamente en onMounted
onMounted(() => {
  currentYear.value = new Date().getFullYear()
})
</script>
