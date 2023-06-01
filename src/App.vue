<template>
  <Navbar />
  <RouterView />
  <FooterComponent />
</template>

<script>
import Navbar from "./components/Navbar.vue"
import FooterComponent from "./components/FooterComponent.vue";
  export default {
    components: {
      Navbar,
      FooterComponent
    },
    mounted () {
      window.scrollTo(0, 0);
    }
  }
</script>

<style scoped>
</style>
