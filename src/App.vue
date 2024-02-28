<script>
export default {
  data() {
    return {
      contador: 0,
    };
  },
  methods: {
    incrementar() {
      this.contador++;
    },
    decrementar() {
      if (this.contador > 0) {
        this.contador--;
      }
    },
    reiniciar() {
      this.contador = 0;
    },
  },
};
</script>

<template>
  <div>
    <h1>Contador</h1>
    <p> {{ contador }} </p>
    <button @click="incrementar">+</button>
    <button @click="decrementar">-</button>
    <button @click="reiniciar">Reiniciar</button>
  </div>
</template>

<style scoped>
button {
  font-weight: bold;
  color: rgb(255, 255, 255);
  background-color: rgb(0, 0, 0);
  border-color: rgb(13, 134, 134);
  border: 4;
}
</style>
