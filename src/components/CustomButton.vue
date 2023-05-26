<template>
    <button type="button">{{ texto }}</button>
</template>

<script>
export default {
    name: "CustomButton",
    props: {
        texto: String
    },
    methods: {
        click() {
            alert("Clicou!");
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>