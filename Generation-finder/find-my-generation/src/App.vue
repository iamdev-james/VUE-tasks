<template>
  <main class= "h-screen bg-blue-100 flex flex-col justify-center items-center">
    <div>
      <input type= 'number' v-model= "generation">
      <input type= 'text' v-model= "gender">
      <button class= 'py-3 px-6' @click= "checkGeneration()"> Submit </button>
    </div>
    <div class= "block">
      This is your clan: {{ gen }}
    </div>
  </main> 
</template>

<script>
import './assets/tailwind.css'
export default {
  name: 'App',
  data() {
    return {
    }
  },
  methods: {
    function generation(x, y) {
    var gen = '';
	  if (x === 0 && (y === 'm' || y === 'f')) {
      gen = "me!"
      } else if (x === 1 || x === -1) {
          if(x === 1 && y === 'm') {
          gen = "son"
          } else if (x === 1 && y === 'f') {
          gen = "daughter"
          } else if (x === -1 && y === 'f') {
          gen = "mother"
          } else if (x === -1 && y === 'm') {
          gen = "father"
          }
        }  else if (x === 2 || x === -2) {
          if(x === 2 && y === 'm') {
          gen = "grandson"
          } else if (x === 2 && y === 'f') {
          gen = "granddaughter"
          } else if (x === -2 && y === 'f') {
          gen = "grandmother"
          } else if (x === -2 && y === 'm') {
          gen = "grandfather"
          }
        } else if (x === 3 || x === -3) {
          if(x === 3 && y === 'm') {
          gen = "great grandson"
          } else if (x === 3 && y === 'f') {
          gen = "great granddaughter"
          } else if (x === -3 && y === 'f') {
          gen = "great grandmother"
          } else if (x === -3 && y === 'm') {
          gen = "great grandfather"
          };
        } else {
        gen = "Unknown x!!!"
      }
    return gen;
    }; 
  }
}
</script>
