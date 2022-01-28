<template>
  <v-app>
    <MenuClone />
    <v-main>
      <Nuxt />
    </v-main>
    <v-footer width="100%">
     <v-container fluid class="pa-0">
      <v-row>
        <v-col class="pa-0">
          <Footer />
        </v-col>
      </v-row>
    </v-container>
    </v-footer>
  </v-app>
</template>

<script>
 export default {
   name: 'defaultLayout',

  }
</script>

<style scoped>
  .v-footer{padding: 6px 0;}
</style>
