<template>
  <main  class="text-white h-1/5">
    <div id="header" class="flex justify-between items-center w-full">
      <div class="flex justify-center items-center">
        <img class="inline" :src='require("@/assets/images/headerLogo.svg")' />
      </div>
      <div class='w-2/5 flex align-center justify-between'>
        <p>Home</p>
        <p>Features</p>
        <p>Testimonial</p>
        <p>Pricing</p>
      </div>
      <div>
        <button class="text-white px-8 py-3 border-white border-2 rounded-full">Get Started</button>
      </div>
      <!-- <div>
        <img :src="require('@/assets/images/Header/navdark.png')" height="10px" />
        <img :src="require('@/assets/images/Header/navwhite.png')" height="1px" />
      </div> -->
    </div>
  </main>
</template>

<script>
export default {
  name: 'HeaderComponent'
}
</script>

<style>
  #header {
    height: 10vh;
  }
</style>