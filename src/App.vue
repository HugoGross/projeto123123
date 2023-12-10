<script>
export default {
  data() {
    return {
      contador: 0
    }
  },
  methods: {
    incrementarContador() {
      this.contador++
    },
    decrementarContador() {
      this.contador--
    }
  },
  mounted() {
    console.log(`O valor inicial do contador é ${this.contador}.`)
  }
}
</script>

<template>
<h2>Incremetador/Decrementador de valores</h2>

<button @click="incrementarContador">Incrementar</button>
<button @click="decrementarContador">Decrementar</button>
<p>Valor do contador é {{ contador }}</p>
</template>

<style scoped>
button {
  font-weight: bold;
}
</style>
<style scoped>
h2 {
 text-align: justify;
}
</style>