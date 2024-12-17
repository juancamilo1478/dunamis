<template>
    <div class="flex flex-col md:flex-row w-full px-3 pt-16 pb-16" style="background: var(--primaty-color);">
        <!-- Contenido de la izquierda -->
        <div class="w-full px-20 flex flex-col justify-center">
            <h1 class="text-white font-nunito font-black text-2xl md:text-4xl lg:text-5xl">Diseñamos tu vision</h1>
            <p class="text-white font-nunito font-medium text-2xl pt-7 leading-relaxed md:text-3xl md:pe-28">
                En <strong style="color: var(--segundaty-color);">Dunamis</strong>, ayudamos a pequeñas y medianas empresas, emprendedores y particulares a destacar en el mundo digital y visual.
            </p>
            <div class="w-1/2 rounded-lg flex justify-center items-center mt-20" style="background: var(--segundaty-color);">
                <h1 class="text-3xl p-3 text-white font-nunito font-bold">Contactar</h1>
            </div>
        </div>
        <!-- Contenido de la derecha (imagen) -->
        <div class="w-full p-4 flex justify-center items-center  md:block">
            <img src="@/assets/photo1.png" alt="Descripción de la imagen" />
        </div>
    </div>
</template>
<script>
export default {
    name:"firstComponent",
}
</script>