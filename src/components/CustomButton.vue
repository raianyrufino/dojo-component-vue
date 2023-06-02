<template>
    <button type="button" class="default" :class="[classes]" >{{ texto }}</button>
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
    },
    computed: {
        classes() {
            return {
                ['default__primario']: this.type === 'primario',
                ['default__secundario']: this.type === 'secundario',
            }
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
.default {
    width: 100px;
    height: 30px;

    &__primario {
        background-color: blue;
        color: white;
    }
    &__secundario {
        background-color: green;
    }
}
</style>