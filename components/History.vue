<template>
  <div class="History">
     <v-container fluid>
      <v-row justify="center">
        <v-col cols="10" xs="10" sm="8" md="3" lg="3" xl="3">
          <div class="HistoryTitle">
            <p>History</p>
            <h1>끊임없는 도전정신과 멈추지 않는 열정이 가득한 NUXT</h1>
          </div>
        </v-col>
        <v-col cols="12" xs="12" sm="8" md="5" lg="5" xl="5" class="timeLineSet">
          <v-timeline dense>
            <v-timeline-item
              v-for="(year, i) in years"
              :key="i"
              :color="year.color"
              small
              fill-dot
              id="tagetSet"
              :class="`${year.atclass}`"
            >
              <div class="py-4">
                <span :class="`headline font-weight-bold mb-4 ${year.color}--text`" v-text="year.year">
                </span>
                <div class="subjectText">{{year.subject}}</div>
              </div>
            </v-timeline-item>
          </v-timeline>
        </v-col>
      </v-row>
     </v-container>
  </div>
</template>

<script>
export default {
  name: 'History',
  data: () => ({
    years: [
      {
        atclass: 'shadow',
        color: '#72c09f',
        year: '2022',
        subject: '독일 히든챔피언 한국지사 글로벌 기업매칭 프로그램 진행',
      },
      {
        atclass: 'shadowNo',
        color: '#e0e0e0',
        year: '2021',
        subject: '2독일 히든챔피언 한국지사 글로벌 기업매칭 프로그램 진행',
      },
      {
        atclass: 'shadowNo',
        color: '#e0e0e0',
        year: '2020',
        subject: '3독일 히든챔피언 한국지사 글로벌 기업매칭 프로그램 진행',
      },
      {
        atclass: 'shadowNo',
        color: '#e0e0e0',
        year: '2019',
        subject: '4독일 히든챔피언 한국지사 글로벌 기업매칭 프로그램 진행',
      },
    ],
  }),
}
</script>

<style scoped>
  .timeLineSet {padding: 0 70px;}
  .History{background: #fafafc; padding: 110px 0;}
  .HistoryTitle p {font-weight: 700; font-size: 1.5rem; line-height: 2.125rem; color: #a2a2a2; margin-bottom: 8px;}
  .HistoryTitle h1 {font-weight: 700; font-size: 2.5rem; line-height: 4rem; color: #333;}
  .subjectText { font-size: 1rem; line-height: 30px; color: #a2a2a2;}
  @media (min-width: 605px){
    .History{padding: 110px 0;}
    .timeLineSet {padding: 0 70px;}
    .HistoryTitle p {font-size: 1.5rem;}
    .HistoryTitle h1 {font-size: 2.5rem; line-height: 4rem;}
  }
  @media (max-width: 960px){
    .History{padding: 40px 0 60px;}
    .timeLineSet{padding: 0 50px 0 10px;}
    .HistoryTitle p {font-size: 1.2rem;}
    .HistoryTitle h1 {font-size: 1.9rem; line-height: 3rem;}
  }
</style>
