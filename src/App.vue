<template>

  <div id="example1">
    <h1>Eu cliquei : {{ contador }}</h1>
    <button @click="somar()">Clique!</button>
  </div>
</template>
 
<script>

export default {
  data: () => ({
    contador: 0,
  }),
  methods: {
    somar() {
      this.contador++;
    },
    limpar() {
      this.contador--
    }
  },
};

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  text-align: center;
  margin-top: 60px;
}
button{
  background-color: red;
  border-radius: 30px;
  padding: 20px;
  font-size: 30px;
}
</style>
