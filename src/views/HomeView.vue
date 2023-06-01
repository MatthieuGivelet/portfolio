<template>
  <HeaderComponent />
  <ApercusProjetComponent />
  <AboutComponent />
  <FormulaireComponent />
</template>

<script>
import AboutComponent from "../components/AboutComponent.vue";
import ApercusProjetComponent from "../components/ApercusProjetComponent.vue";
import HeaderComponent from "../components/HeaderComponent.vue"
import FormulaireComponent from "../components/FormulaireComponent.vue";
  export default {
    components: {
      HeaderComponent,
      ApercusProjetComponent,
      AboutComponent,
      FormulaireComponent
    }
  }
</script>

<style>
</style>