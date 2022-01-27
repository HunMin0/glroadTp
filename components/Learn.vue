<template>
  <div class="Learn">
    <div class="PromotionTitle">
      <h1>NUXT <span>서비스</span> 더 알아보기</h1>
      <p>기업의 정보를 안전하게 관리하면서도 쉽고 빠르게 소통하세요.</p>
    </div>
     <v-container>
      <v-row align="center" justify="center">
        <v-col cols="10" xs="10" sm="10" md="8" lg="8" xl="6" class="text-center">
          <v-row>
            <v-col cols="12" class="colPosition">
              <v-img height="250" src="/cat-1.jpg">
              <div class="imgTitle">
                <h3>서비스 비전</h3>
                <p>서비스 자원을 이동하여 새로운 경제를 창출합니다.</p>
              </div>
              </v-img>
            </v-col>
          </v-row>
          <v-row>
            <v-col cols="12" xs="12" sm="6" md="6" lg="6" xl="6" class="colPosition">
              <v-img height="250" src="/cat-2.jpg">
               <div class="imgTitle">
                <h3>인사말</h3>
                <p>모든 세상의 움직임은 네트워크로 통합니다.</p>
              </div>
              </v-img>
            </v-col>
            <v-col cols="12" xs="12" sm="6" md="6" lg="6" xl="6" class="colPosition">
              <v-img height="250" src="/cat-3.jpg">
               <div class="imgTitle">
                <h3>상담문의</h3>
                <p>서비스 관련 문의를 요청하세요.</p>
              </div>
              </v-img>
            </v-col>
          </v-row>
        </v-col>
        <v-col cols="10" xs="10" sm="10" md="4" lg="4" xl="4" class="colPosition">
          <v-img class="imgBox" src="/cat-4.jpg">
           <div class="imgTitle">
              <h3>서비스 소개</h3>
              <p>NUXT는 어떤 서비스일까요?</p>
            </div>
          </v-img>
        </v-col>
      </v-row>
     </v-container>
  </div>
</template>

<script>
export default {
  name: 'Learn',
  data: () => ({

  }),
}
</script>

<style scoped>
.colPosition {position: relative;}
.imgTitle {width: auto; background: rgb(255 255 255 / 93%); position: absolute; right: 0; bottom: 0; padding: 20px 40px; text-align: left;}
.imgTitle p {margin: 0;}
.Learn {padding: 10px 0 110px;}
.imgBox {height: 524px;}
@media (min-width: 605px){
  .imgBox{height: 524px;}
  .Learn {padding: 10px 0 110px;}
}
@media (max-width: 960px){
  .imgBox{height: 250px;}
  .imgTitle{width: 100%;}
  .Learn {padding: 10px 0 30px;}
}
</style>
