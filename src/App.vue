<template>
  <img alt="Vue logo" src="./assets/logo.png"> 
  
  <custom-button texto="Botão" funcaoClick="click"></custom-button>
</template>

<script>
import CustomButton from './components/CustomButton.vue'

export default {
  name: 'App',
  components: {
    CustomButton,
  },
  methods:{
    click() {
            alert("Clicou!");
        }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

</style>

<!-- Teste -->>