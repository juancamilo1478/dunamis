<script>
import { RouterView } from 'vue-router'
import Navbar from './navbar.vue'
import FirstComponent from "./firsdComponent.vue"
import Services from "./services.vue"
import Proyects from "./Proyects.vue"
export default {
    name:"home",
    components: {
    Navbar,  
    FirstComponent,
    Services,
    Proyects
  },
}
</script>
<template>
    <div class="Style_Main_Home no-gutters">
        <navbar />
        <FirstComponent/>
        <Services/>
        <Proyects/>
      </div>
</template>

<style>
html,
body,
#app {
  margin: 0;
  overflow-y: auto;
  overflow-x: hidden;
  width: 100%;
  min-height: 100vh;
  background: var(--terseary-color);
  padding: 0;
  font-family: "Nunito", sans-serif;
  font-optical-sizing: auto;
  font-weight: 400;
  
  background-color: var(--primary-color);
}

.Style_Main_Home {
  width: 100%;
  background-color: var(--terseary-color);
  display: block;
  min-height: 100vh;
}
</style>
