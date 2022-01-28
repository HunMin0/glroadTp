<template>
  <div class="logo" v-bind:title="logoName">
   <v-img height="54px" src="/logo.png" contain></v-img>
  </div>
</template>

<script>
export default {
  name: 'Logo',
  data: () => ({
    logoName:'NUXT HOME',
  }),
}
</script>

<style scoped>
.logo {padding-top: 10px;}
.nuxt-logo {height: 30px;}
.logo span {color:#333; padding-left: 10px;}
</style>
