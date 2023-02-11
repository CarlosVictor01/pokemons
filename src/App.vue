<template>
  <div>
    <Header :title="titleText" :subtitle="subtitleText"/>
    <SeachBar/>
  </div>
</template>

<script>
import Header from "./components/header.vue";
import SeachBar from "./components/seachBar.vue";

export default {

  data() {
    return {
      titleText: 'Pokesearch',
      subtitleText: 'Procure seu pokémon favorito e descubra suas habilidades',
      names: []
    }
  },

  components: {
    Header,
    SeachBar
},
}
</script>

<style>

</style>
