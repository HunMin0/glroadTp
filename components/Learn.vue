<template>
  <div class="Learn">
    <div class="PromotionTitle">
      <h1>NUXT <span>서비스</span> 더 알아보기</h1>
      <p>기업의 정보를 안전하게 관리하면서도 쉽고 빠르게 소통하세요.</p>
    </div>
     <v-container>
      <v-row align="center" justify="center" no-gutters>
        <v-col cols="10" xs="10" sm="10" md="8" lg="8" xl="6" class="text-center">
          <v-row no-gutters>
            <v-col cols="12" class="colPosition" title="서비스비전">
              <div id="sector1">
                <router-link to="/">
                  <v-img class="imgBox" height="250" src="/cat-1.jpg"></v-img>
                  <div class="imgTitle">
                    <h3>서비스 비전</h3>
                    <p>서비스 자원을 이동하여 새로운 경제를 창출합니다.</p>
                  </div>
                </router-link>
              </div>
            </v-col>
          </v-row>
          <v-row no-gutters>
            <v-col cols="12" xs="12" sm="6" md="6" lg="6" xl="6" class="colPosition sad" title="인사말">
               <div id="sector2">
                 <router-link to="/">
                  <v-img class="imgBox" height="250" src="/cat-2.jpg"></v-img>
                  <div class="imgTitle">
                    <h3>인사말</h3>
                    <p>모든 세상의 움직임은 네트워크로 통합니다.</p>
                  </div>
                  </router-link>
              </div>
            </v-col>
            <v-col cols="12" xs="12" sm="6" md="6" lg="6" xl="6" class="colPosition" title="상담문의">
              <div id="sector3">
               <router-link to="/">
                <v-img class="imgBox" height="250" src="/cat-3.jpg"></v-img>
                <div class="imgTitle">
                  <h3>상담문의</h3>
                  <p>서비스 관련 문의를 요청하세요.</p>
                </div>
                </router-link>
              </div>
            </v-col>
          </v-row>
        </v-col>
        <v-col cols="10" xs="10" sm="10" md="4" lg="4" xl="4" class="colPosition" title="서비스소개">
          <v-row no-gutters>
            <v-col>
              <div id="sector4">
                <router-link to="/">
                  <v-img class="imgBox" src="/cat-4.jpg"></v-img>
                  <div class="imgTitle">
                    <h3>서비스 소개</h3>
                    <p>NUXT는 어떤 서비스일까요?</p>
                  </div>
                </router-link>
              </div>
            </v-col>
          </v-row>
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

.paddingSet {padding: 12px }
.colPosition {position: relative; overflow: hidden;}
.colPosition .imgBox {transition: all 0.5s;}
.colPosition:hover .imgBox {transform: scale(1.6); transition: all 1s;}
.colPosition a {color: #333;}
.imgTitle {width: auto; background: rgb(255 255 255 / 93%); position: absolute; right: 0; bottom: 0; padding: 20px 40px; text-align: left;}
.imgTitle p {margin: 0;}
.Learn {padding: 10px 0 110px;}
.imgBox {height: 524px;}

#sector1{width: 856px; height: 250px; overflow: hidden; margin: 12px; position: relative;}
#sector2{width: 416px; height: 250px; overflow: hidden; margin: 12px; position: relative;}
#sector3{width: 416px; height: 250px; overflow: hidden; margin: 12px; position: relative;}
#sector4{width: 565px; height: 524px; overflow: hidden; margin: 12px; position: relative;}

@media (min-width: 1904px){
  #sector1{width: 856px;}
  #sector2{width: 416px;}
  #sector3{width: 416px;}
  #sector4{width: 565px;}
}
@media (min-width: 1261px){
  #sector1{width: 100%;}
  #sector2{width: 100%;}
  #sector3{width: 100%;}
  #sector4{width: 100%;}
  .imgBox{height: 524px;}
  .Learn {padding: 10px 0 110px;}
  .imgTitle {padding: 20px; left: unset;}
}
@media (max-width: 1260px){
  #sector1{width: 100%;}
  #sector2{width: 100%;}
  #sector3{width: 100%;}
  #sector4{width: 100%;}
  .imgBox{height: 524px;}
  .Learn {padding: 10px 0 110px;}
  .imgTitle {padding: 20px; left: 0;}
  .imgTitle h3 {font-size: 18px;}
  .imgTitle p {font-size: 14px;}
}
@media (max-width: 960px){
  #sector1{width: 100%;}
  #sector2{width: 100%;}
  #sector3{width: 100%;}
  #sector4{width:100%; height: 250px;}
  .imgBox{height: 250px;}
  .imgTitle{width: 100%;}
  .Learn {padding: 10px 0 30px;}
}
</style>
