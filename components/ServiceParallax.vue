<template>
  <div class="ServiceParallax">
    <v-parallax dark src='/parallax.jpg' height="400">
     <v-container fluid>
      <v-row align="center" justify="center">
        <v-col cols="5" xs="5" sm="5" md="2" lg="2" xl="2" class="text-center"
          v-for="(item,i) in items"
          :key="i"
        >
          <v-icon x-large color="#fff">{{item.icon}}</v-icon>
          <h1 class="textStyle">{{item.firstTitle}}</h1>
          <h4 class="subheading">{{item.subject}}</h4>
        </v-col>
      </v-row>
     </v-container>
    </v-parallax>
  </div>
</template>

<script>
export default {
  name: 'ServiceParallax',
  data: () => ({
     items: [
      {
        icon: 'mdi-package-variant-closed',
        firstTitle: '2만건+',
        subject: 'GLROAD 수출진행건수'
      },
       {
        icon: 'mdi-database',
        firstTitle: '800억+',
        subject: '수출 규모'
      },
       {
        icon: 'mdi-timetable',
        firstTitle: '3일+',
        subject: '평균 업무시간'
      },
       {
        icon: 'mdi-timer',
        firstTitle: '30분+',
        subject: '평균 매칭소요시간'
      },
    ],
  }),
}

</script>

<style scoped>
  .textStyle{margin: 10px 0; font-size: 2.7rem;}
  .subheading{font-size: 1rem; font-weight: 400;}
  @media (min-width: 605px){
    .textStyle{font-size: 2.7rem;}
  }
  @media (max-width: 960px){
    .textStyle{font-size: 1.7rem;}
  }
</style>
