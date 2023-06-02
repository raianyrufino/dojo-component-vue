<template>
    <button type="button" :class="[classes]">{{ texto }}</button>
</template>

<script>
export default {
    name: "CustomButton",
    props: {
        texto: String,
        type: String,
    },
    methods: {
        click() {
            alert("Clicou!");
        }
    }
    computed: {
        classes() {
            return {
                ['primario']: this.type === 'primario',
                ['secundario']: this.type === 'secundario',
            }
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
 .primario {
    background-color: blue;
 }
 .secundario {
    background-color: green;
 }
</style>