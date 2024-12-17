<template>
    <div class="w-[500px] rounded-lg  ">
      <!-- Card del proyecto -->
      <img :src="proyect.images[0]" alt="Imagen del proyecto" class="w-full rounded-t-lg" />

      <div
        class="  p-6  shadow-lg "
         style="background: var(--primaty-color);"
      >
        <h2 class="  font-bold text-white font-nunito text2">{{ proyect.name }}</h2>
        <p class="text-gray-700">{{ proyect.description }}</p>
        
      </div>
      <div class="w-full rounded-b-lg  cursor-pointer" style="background: var(--segundaty-color);"  @click="showModal = true">
        <h1 class="p-4 flex justify-center items-center text-white font-nunito font-bold text-2xl">Ver más</h1>
    </div>
    
      <!-- Modal -->
      <div
        v-if="showModal"
        class="fixed inset-0 flex items-center justify-center bg-black bg-opacity-50"
      >
        <div class="bg-white p-8 rounded-lg shadow-lg w-3/4 md:w-1/2">
          <h2 class="text-2xl font-bold mb-4">{{ proyect.name }}</h2>
          <p class="text-gray-700 mb-6">{{ proyect.description }}</p>
          <button
            class="px-4 py-2 bg-red-500 text-white rounded hover:bg-red-600"
            @click="showModal = false"
          >
            Cerrar
          </button>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "Item",
    props: {
      proyect: {
        type: Object,
        required: true,
      },
    },
    data() {
      return {
        showModal: false, // Controla la visibilidad del modal
      };
    },
  };
  </script>
  
  <style scoped>
  /* Estilos adicionales opcionales */
  </style>
  