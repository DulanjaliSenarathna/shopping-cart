<template>
  <div >
    <Cart/>
    <RouterView/>
  </div>
</template>

<script setup> 
    import {RouterView} from "vue-router";
    import Cart from "./components/Cart.vue";
</script>

<style lang="scss" scoped>

</style>