<script>
export default {
  data: () => ({ 
    contador: 10, }),
  methods: {
    incrementar() {
      this.contador++;
    },
    disminuir() {
      this.contador--;
    },
    resetear() {
      this.contador=10;
    },
  },
};
</script>


<template>
  <div class="container">
    <img src="./assets/logo.svg" alt="LOGO VUE" width="125" height="125" />
    <small><h1>Hola Soy Paniagua y este es mi primer contador</h1> </small>
    <hr />

    <h2>Contador: {{ contador }}</h2>
    <button @click="incrementar()">+1</button>
    <button @click="disminuir()">-1</button>
    <button @click="resetear()">Reset</button>
  </div>
</template>
