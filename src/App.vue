<template>
  <div>
    <div class="align-center">
      <h1>{{ titulo }}</h1>
    </div>
    <div>
      <ul>
        <li v-for="name in names">
          {{ names }}
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {

  data() {
    return {
      titulo: 'POKEMONS',
      names: []
    }
  }, 

  created() {
    this.$http.get('https://pokeapi.co/api/v2/pokemon/')
      .then(res => res.json())
      .then(name => this.names = name);
  }
}
</script>

<style>
</style>
