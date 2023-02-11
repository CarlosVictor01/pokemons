<template>
    <button class="btn">
        {{ btnText }}
    </button>
</template>

<script>
export default {
    name: 'Button',
    props: {
        btnText: String
    },
}

</script>

<style>
.btn {
    position: relative;
    background-color: #4CAF50;
    font-size: 15px;
    color: #FFFFFF;
    padding: 12px;
    width: 150px;
    text-align: center;
    transition-duration: 0.4s;
    text-decoration: none;
    overflow: hidden;
    cursor: pointer;
    margin: 8px 0;
    display: inline-block;
    border: 1px solid #ccc;
    border-radius: 4px;
    box-sizing: border-box;
}
</style>