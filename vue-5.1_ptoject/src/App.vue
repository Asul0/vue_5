<template>
  <div id="app">
    <ProductDetails />
  </div>
</template>

<script>
import ProductDetails from './components/ProductDetails.vue';

export default {
  name: 'App',
  components: {
    ProductDetails
  }
};
</script>

<style>
#app {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  background-color: #e0e0e0;
  margin: 0;
  font-family: Arial, sans-serif;
}
</style>
