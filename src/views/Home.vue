<template>
  <div>
  <Banner />
  <div class="main-container">
    <h1>Monte o seu burger:</h1>
    <BurgerForm />
  </div>
</div>
</template>

<script>
import Banner from '@/components/Banner.vue';
import BurgerForm from '@/components/BurgerForm.vue';
export default {
  name: 'Home',
  components: {
    Banner,
    BurgerForm
  }
}
</script>

<style>
h1::selection {
  background-color: #fcba03;
}
</style>