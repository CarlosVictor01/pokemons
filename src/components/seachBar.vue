<template>
    <section class="container">
        <form @submit="onSubmit" class="teste">
            <input class="inputName"
                placeholder="Insira o nome de um Pokemon"
                name="pokemoName"
                type="text"
                v-model="pokemoName"
            />
            <Button :btnText="btnText" type="submit"/>
        </form>
    </section>
</template>

<script>
import Button from './button.vue';

export default {
    name: 'SeachBar',
    data() {
        return {
            pokemoName: "",
            btnText: "Buscar"
        }
    },

    components: {
        Button
    }, 

    methods: {
        onSubmit(e) {
            e.preventDefault();
            this.$emit("search_pokemoName", this.pokemoName);
        }
    }
}

</script>

<style>
.container {
    width: 100%;
    height: 7vh;
    padding: 3rem 0;
    background: lightblue;
}

.inputName {
    width: 20%;
    padding: 12px 20px;
    margin: 8px 0;
    display: inline-block;
    border: 1px solid #ccc;
    border-radius: 4px;
    box-sizing: border-box;
}

.teste {
    display: flex;
    align-items: center;
    justify-content: center;
}
</style>