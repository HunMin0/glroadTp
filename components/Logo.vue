<template>
  <div class="logo" v-bind:title="logoName">
   <v-img height="54px" src="/logo2.png" contain></v-img>
  </div>
</template>

<script>
export default {
  name: 'Logo',
  data: () => ({
    logoName:'GLROAD HOME',
  }),
}
</script>

<style scoped>
.nuxt-logo {height: 30px;}
.logo span {color:#fff; padding-left: 10px;}
</style>
