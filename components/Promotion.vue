<template>
  <div class="Promotion">
    <div class="PromotionTitle">
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
     <v-row
       align="center"
       justify="center"
      >
       <v-col
          cols="10" xs="10" sm="10" md="10" lg="9" xl="6"
          class="text-right"
        >
          <router-link to="/"><p class="lastArea" title="자세히보기">NUXT에 대해 더 알아보기 <v-icon>mdi-arrow-top-right</v-icon></p></router-link>
        </v-col>
     </v-row>
  </div>
</template>

<script>
export default {
  name: 'Promotion',
  data: () => ({
    items: [
      {
        imgIcon: '/icon01.png',
        firstTitle: '신뢰할 수 있는 클라우드 인프라',
        subject: '세계 최고 수준의 보안과 안정적인 인프라를 제공하는 AWS기반 운영',
        lastText: '모든 메시지와 파일 전송 즉시 암호화 처리'
      },
      {
        imgIcon: '/icon02.png',
        firstTitle: '2신뢰할 수 있는 클라우드 인프라',
        subject: '세계 최고 수준의 보안과 안정적인 인프라를 제공하는 AWS기반 운영',
        lastText: '모든 메시지와 파일 전송 즉시 암호화 처리'
      },
      {
        imgIcon: '/icon03.png',
        firstTitle: '3신뢰할 수 있는 클라우드 인프라',
        subject: '세계 최고 수준의 보안과 안정적인 인프라를 제공하는 AWS기반 운영',
        lastText: '모든 메시지와 파일 전송 즉시 암호화 처리'
      }
    ],
  }),
}
</script>

<style scoped>
  .Promotion{background: #fafafc; padding: 30px 0 110px;}
  .PromotionTitle{width: 100%; text-align: center;}
  .PromotionTitle span {color:#72c09f}
  .cardStyle{box-shadow: 0 14px 24px rgb(0 18 47 / 8%)!important; border-radius: 24px; padding: 30px 16px;}
  .firstTitle{font-weight: 700; font-size: 1.60rem; line-height: 42px; margin: 24px 0;}
  .subject{font-size: 1rem; line-height: 30px; text-align: center; margin-top: 20px;}
  .lastArea{font-weight: 400; font-size: 1.110rem; line-height: 20px; color: #a2a2a2; margin: 25px 10px 0 0;}
  .lastArea i {color: #a2a2a2;}

  @media (min-width: 605px){
    .firstTitle{font-size: 1.60rem;}

  }
  @media (max-width: 960px){
    .firstTitle{font-size: 1.40rem;}
    .PromotionTitle{font-size: 0.9rem;}
  }
</style>
