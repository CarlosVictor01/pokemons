<template>
  <div>
    <Header :title="titleText" :subtitle="subtitleText"/>
  </div>
</template>

<script>
import Header from "./components/header.vue";
export default {

  data() {
    return {
      titleText: 'Pokesearch',
      subtitleText: 'Search for your favorite pokemon',
      names: []
    }
  },

  components: {
    Header
  },
}
</script>

<style>

</style>
