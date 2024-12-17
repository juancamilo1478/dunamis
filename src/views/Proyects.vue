<template>
    <div class="w-full px-20 py-8">
        <h1 class="text-white text-5xl font-nunito font-bold">Proyectos</h1>
        <div class="w-full flex flex-wrap gap-10 justify-center items-stretch pb-40 pt-32">
            <Item v-for="proyect in proyectdata" :key="proyect.id" :proyect="proyect"  />
        </div>
    </div>
</template>

<script>
import proyectdata from '@/assets/data.json';
import Item from './Item.vue';

export default {
    name: 'Proyects',
    components: { // Debe ser "components" y no "componente"
        Item
    },
    data() {
        return {
            proyectdata: proyectdata // Asignamos los datos del JSON a una propiedad del componente
        };
    }
};
</script>