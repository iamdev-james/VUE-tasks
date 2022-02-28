<template>
  <v-bottom-navigation
    :value="value"
    color="teal"
    grow
  >
    <v-btn>
    </v-btn>
      <h2>devfinder</h2>
    <v-spacer></v-spacer>
    <v-btn>
      <span>Light</span>
      <v-icon>mdi-map-marker</v-icon>
    </v-btn>
  </v-bottom-navigation>
</template>

<script>

export default {
  name: 'App',
  data: () => ({
    //
  })
}
</script>
