<template>
  <div>
    <Header :title="titleText" :subtitle="subtitleText"/>
    <SeachBar @search_pokemoName="getPokemons" />
  </div>
</template>

<script>
import Header from "./components/header.vue";
import SeachBar from "./components/seachBar.vue";
import { IEvolutionChain, IPokemon } from "./utils/interfaces";

export default {
  name: "App",
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

  methods: {
  }
}
</script>

<style>

</style>
