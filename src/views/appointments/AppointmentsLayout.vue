<script setup lang="ts"></script>

<template>
  <div class="flex justify-between">
    <h1 class="text-2xl lg:text-6xl font-black text-white">Barbería</h1>
    <div class="flex flex-col space-y-5">
      <div class="flex gap-2 items-center">
        <p class="text-white text-right">Hola: Usuario</p>

        <button
          type="button"
          class="bg-red-600 hover:bg-red-700 p-2 text-white uppercase text-xs font-extrabold rounded-lg transition-all"
        >
          Cerrar Sesión
        </button>
      </div>
      <nav class="flex gap-2 items-center justify-end">
        <button class="p-3 text-gray-200 uppercase text-xs font-black rounded-lg">Mis Citas</button>
        <RouterLink
          :to="{ name: 'new-appointment' }"
          class="bg-blue-700 hover:bg-blue-800 p-3 text-gray-200 uppercase text-xs font-black rounded-lg transition-all"
          >Nueva Cita</RouterLink
        >
      </nav>
    </div>
  </div>
  <main>
    <RouterView />
  </main>
</template>
