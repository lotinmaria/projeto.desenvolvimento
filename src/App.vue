<script setup>
import { ref } from 'vue'

const contador = ref(0)

function decrementar(){
  if (contador.value >0){contador.value--}
}

function reset(){
  contador.value = 0
  
}

</script>

<template> 
<button @click="contador++">+</button>
<button @click="decrementar">-</button>
<button @click="reset">reset</button>
<p> valor do contador: {{ contador }}</p>
</template>

<style scoped>
button {
  font-weight: bold;
  color: rgb(3, 90, 18);
  background-color: rgb(22, 201, 156);
  border: 2;
}</style>
