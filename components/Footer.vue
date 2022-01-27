<template>
  <v-container fluid class="footerBg">
    <v-row align="center" justify="center" class="fotterLine">
      <v-col cols="12" xs="12" sm="12" md="12" lg="12" xl="8">
        <div class="footerTerms">
          <ul class="pa-0">
            <li title="회사소개"> <router-link to="/">회사소개</router-link></li>
            <li><span>I</span></li>
            <li title="서비스이용약관"> <router-link to="/">서비스이용약관</router-link></li>
            <li><span>I</span></li>
            <li title="개인정보처리방침"> <router-link to="/">개인정보처리방침</router-link></li>
            <li><span>I</span></li>
            <li title="이메일무단수집거부"> <router-link to="/">이메일무단수집거부</router-link></li>
          </ul>
        </div>
      </v-col>
    </v-row>
    <v-row align="center" justify="center">
      <v-col cols="12" xs="12" sm="12" md="12" lg="12" xl="8">
        <div class="footer">
          <ul class="pa-0">
            <li><!--<v-img height="64px" src="/logo2.png" contain></v-img>-->로고</li>
            <li>대표 : 홍길동&emsp;<span>I</span>&emsp;주소 : 대전시 서구 둔산남로11-1(둔산동,NUXT빌딩)&emsp;<span>I</span>&emsp;TEL : 042-123-4567&emsp;<span>I</span>&emsp;Fax : 042-123-4567&emsp;<span>I</span>&emsp;E-Mail : custorm_cs@gmail.com
              <br/><span>Copyright © 2022 NUXTSOFT All rights reserved.</span>
            </li>
          </ul>
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'Footer',
  data: () => ({
    items: [
      {

      },
    ],
  }),
}
</script>

<style scoped>
  .footerBg{background: #2b2f3b; text-align: center; padding: 0 40px;}
  .fotterLine {border-bottom: 1px solid #4c4d4e;}
  .footerTerms ul li {color: #b7b7b7; display: inline-block; list-style: none; font-size: 0.875rem; padding: 6px 14px;}
  .footerTerms ul li span {color:#777b85}
  .footer {padding: 20px 0;}
  .footer ul li {color: #a7a6a6; list-style: none; font-size: 0.938rem;  line-height: 2.125rem;}
  .footer ul li span {color: #777b85;}
  .footer ul li:first-child {margin-bottom: 10px;}
  .v-application a{color:#b7b7b7;}
  @media (min-width: 605px){
    .footerTerms ul li{padding: 6px 14px; font-size: 0.875rem;}
  }
  @media (max-width: 960px){
    .footerTerms ul li{padding: 6px 2px; font-size: 0.800rem;}
  }
</style>
