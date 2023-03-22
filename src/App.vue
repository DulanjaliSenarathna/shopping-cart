<template >
  <div id="app" class="flex flex-col min-h-screen  bg-[#F0EEED]">
    <Cart/>
    <RouterView/>
  </div>
</template>

<script setup> 
    import {RouterView} from "vue-router";
    import Cart from "./components/Cart.vue";
</script>
