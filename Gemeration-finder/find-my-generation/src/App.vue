<template>
  <main class= "h-screen bg-blue-100 flex flex-col justify-center items-center">
    <div>
      <input type= 'number' v-model= "generation">
      <input type= 'text' v-model= "gender">
      <button class= 'py-3 px-6' @click= "checkGeneration()"> Submit </button>
    </div>
    <div class= "block">
      This is your clan: {{ gen_name }}
    </div>
  </main> 
</template>

<script>
import './assets/tailwind.css'
export default {
  name: 'App',
  data() {
    return {
      gen_name: '',
      generationvalue: Number,
      gendervalue: ''
    }
  },
  methods: {
    checkGeneration() {
      this.generation(this.generationvalue, this.gendervalue)
    },
    generation (generation, gender) {
      if (generation === 0 && gender === 'M' || gender === 'F') {
        this.gen_name = 'me!'
        return
      } else if (generation === 1 || generation === -1) {
          if(generation === 1 && gender === 'm') {
            this.gen_name = 'son'
          } else if (generation === 1 && gender === 'f') {
            this.gen_name = 'daugther'
          } else if (generation === -1 && gender === 'f') {
            this.gen_name = 'mother'
          } else if (generation === -1 && gender === 'm') {
            this.gen_name = 'father'
          }
      }  else if (generation === 2 || generation === -2) {
          if(generation === 2 && gender === 'm') {
            this.gen_name = 'grandson'
          } else if (generation === 2 && gender === 'f') {
            this.gen_name = 'granddaugther'
          } else if (generation === -2 && gender === 'f') {
            this.gen_name = 'grandmother'
          } else if (generation === -2 && gender === 'm') {
            this.gen_name = 'grandfather'
          }
      } else if (generation === 3 || generation === -3) {
          if(generation === 3 && gender === 'm') {
            this.gen_name = 'great grandson'
          } else if (generation === 3 && gender === 'f') {
            this.gen_name = 'great granddaugther'
          } else if (generation === -3 && gender === 'f') {
            this.gen_name = 'great grandmother'
          } else if (generation === -3 && gender === 'm') {
            this.gen_name = 'great grandfather'
          }
      } else {
          this.gen_name = "Unknown generation!!!"
      }
    } 
  }
}
</script>
