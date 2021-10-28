<template>
  <div id="app">

      <h1>Bem vindo ao meu primeiro projeto!</h1>
      <button @click="entrar">Entrar</button>

      <Usuario nome="Fi"/>
      <Usuario :nome="nome"/>

  </div>
  
</template>

<script>
import Usuario from './components/Usuario';
  export default {
    name: 'App',
    components: {
      Usuario
    },
    data(){
      return {
        nome: 'Sujeito programador'
      }
    },
    methods:{
      entrar(){
        this.nome = 'Curso Vue Js';
      }
    }
  }
</script>

<style>


</style>