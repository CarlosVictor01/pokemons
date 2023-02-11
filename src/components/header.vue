<template>
    <header class="top">
        <h1 class="title">
            {{ title }}
        </h1>
        <h4 class="subtitle">
            {{ subtitle }}
        </h4>
    </header>
</template>

<script>
export default {
    name: "header",
    props: {
        title: String,
        subtitle: String
    }
}
</script>

<style>
.top {
    background-color: lightgreen;
    padding: 2rem 0;
    height: 10%;  
}
.title {
    color: black;
    text-align: center;
    font-family:Georgia, 'Times New Roman', Times, serif;
    font-size: 300%;
}
.subtitle {
    color: darkgreen;
    text-align: center;
}
</style>