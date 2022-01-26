<template>
  <div class="Learn">
    <div class="LearnTitle">
      <h1>강력한 <span>보안</span> 위 풍부한 소통</h1>
      <p>기업의 정보를 안전하게 관리하면서도 쉽고 빠르게 소통하세요.</p>
    </div>
     <v-container fluid>
      <v-row
          align="center"
          justify="center"
        >
        <v-col
          cols="10" xs="10" sm="10" md="10" lg="3" xl="2"
          class="text-center"
          v-for="(item,i) in items"
          :key="i"
        >
          <v-card
            class="cardStyle"
            elevation="0"
            max-height="494"
          >
            <v-card-text>
              <div>
                <v-img
                :src="item.imgIcon"
                :height="100"
                contain
              ></v-img>
              </div>
              <p class="firstTitle">
                {{item.firstTitle}}
              </p>
              <p class="subject">
                {{item.subject}}
              </p>
              <div class="subject">
                {{item.lastText}}
              </div>
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
     </v-container>
  </div>
</template>

<script>
export default {
  name: 'Learn',
  data: () => ({
    items: [
      {
        imgIcon: '/icon01.png',
        firstTitle: '신뢰할 수 있는 클라우드 인프라',
        subject: '세계 최고 수준의 보안과 안정적인 인프라를 제공하는 AWS기반 운영',
        lastText: '모든 메시지와 파일 전송 즉시 암호화 처리'
      },
    ],
  }),
}
</script>

<style scoped>


  @media (min-width: 605px){

  }
  @media (max-width: 960px){

  }
</style>
