<template>

<div>

  <Visual />
  <v-container fluid id="about">
    <v-row>
      <v-spacer/>
      <v-col cols="12" xs="12" sm="12" md="12" lg="10" xl="8">
        <AboutSlid />
      </v-col>
      <v-spacer/>
    </v-row>
  </v-container>


</div>

</template>

<script>
export default {
  name: 'indexPage',
  layout: 'defaultLayout'

}
</script>

<style scoped>

</style>
