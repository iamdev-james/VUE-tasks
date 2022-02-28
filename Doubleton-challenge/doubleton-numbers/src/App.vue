<template>
   <main>
     Doubleton Numbers
   </main>
</template>

<script>
export default {
  name: 'App',
  methods: {
    doubleton(n){
      let s = n + 1
      const number = String(s);
      while (new Set(number).size!==2) {
        s++
      }
    }
  }
}
</script>

<style>

</style>
