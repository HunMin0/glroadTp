<template>
  <div class="aboutSlid">
    <div class="aboutTitle">
      <p>「누구나 쉽게 수출 할 수 있는 <span>디지털 NUXT 플랫폼</span>」</p>
      <p>필요한 공간을 검색하고, 실시간 NUXT 스케줄과 서버정보를 체크하고,<br/>
          이 모든 과정이 스마트하게 이루어집니다.<br/>
          모바일에서 진행하는 나의 디지털 NUXT 파트너! NUXT</p>
    </div>
    <v-stepper non-linear flat alt-labels>
        <v-stepper-header>
            <v-stepper-step editable step="1" color="#72c09f" v-ripple="false">
                서버검색
            </v-stepper-step>
                <v-divider></v-divider>
            <v-stepper-step editable step="2" color="#72c09f" v-ripple="false">
                서버결정
            </v-stepper-step>
                <v-divider></v-divider>
            <v-stepper-step editable step="3" color="#72c09f" v-ripple="false">
                서버셋팅
            </v-stepper-step>
                <v-divider></v-divider>
            <v-stepper-step editable step="4" color="#72c09f" v-ripple="false">
                서버완료
            </v-stepper-step>
        </v-stepper-header>
        <v-stepper-items>
            <v-stepper-content step="1">
              <!-- 슬라이드 스텝1 -->
              <v-row>
                <v-col cols="12" xs="12" sm="12" md="7" lg="7" xl="7">
                  <div class="cardImg">
                    <v-img src="/date.png" contain max-height="360"/>
                  </div>
                </v-col>
                <v-col cols="12" xs="12" sm="12" md="5" lg="5" xl="5">
                  <v-card class="mx-auto"  elevation="0">
                  <v-list-item>
                    <v-list-item-content>
                      <v-card-title class="fontStyleTitle">ABOUT US</v-card-title>
                      <v-card-text class="fontStyleH1">실시간 서버 공간 정보 검색</v-card-text>
                      <v-card-subtitle class="fontStyleH2">아래 세 가지 정보만을 입력 하여 서버공간의 <span>스케줄 및 최저가를 빠르게 검색</span> 할 수 있습니다.</v-card-subtitle>
                      <v-card-text>
                        <ul class="listStyle">
                          <li><v-icon dense>mdi-arrow-right-drop-circle-outline</v-icon> 이동하고자 하는 로컬 호스트</li>
                          <li><v-icon dense>mdi-arrow-right-drop-circle-outline</v-icon> 이동하고자 하는 로컬 호스트</li>
                          <li><v-icon dense>mdi-arrow-right-drop-circle-outline</v-icon> 이동하고자 하는 로컬 호스트</li>
                        </ul>
                      </v-card-text>
                      <v-card-actions>
                        <v-btn depressed color="accent" width="130px" height="50px">
                          Read More
                        </v-btn>
                      </v-card-actions>
                    </v-list-item-content>
                  </v-list-item>
                  </v-card>
                </v-col>
              </v-row>
              <!-- 스텝1 종료 -->
            </v-stepper-content>
            <v-stepper-content step="2">
              <!-- 슬라이드 스텝2 -->
              <v-row>
               <v-col cols="12" xs="12" sm="12" md="7" lg="7" xl="7">
                  <div class="cardImg">
                    <v-img src="/date.png" contain max-height="360"/>
                  </div>
                </v-col>
                <v-col cols="12" xs="12" sm="12" md="5" lg="5" xl="5">
                  <v-card class="mx-auto"  elevation="0">
                  <v-list-item>
                    <v-list-item-content>
                      <v-card-title class="fontStyleTitle">ABOUT US</v-card-title>
                      <v-card-text class="fontStyleH1">실시간 서버 공간 정보 검색</v-card-text>
                      <v-card-subtitle class="fontStyleH2">아래 세 가지 정보만을 입력 하여 서버공간의 <span>스케줄 및 최저가를 빠르게 검색</span> 할 수 있습니다.</v-card-subtitle>
                      <v-card-text>
                        <ul class="listStyle">
                          <li><v-icon dense>mdi-arrow-right-drop-circle-outline</v-icon> 이동하고자 하는 로컬 호스트</li>
                          <li><v-icon dense>mdi-arrow-right-drop-circle-outline</v-icon> 이동하고자 하는 로컬 호스트</li>
                          <li><v-icon dense>mdi-arrow-right-drop-circle-outline</v-icon> 이동하고자 하는 로컬 호스트</li>
                        </ul>
                      </v-card-text>
                      <v-card-actions>
                        <v-btn depressed color="accent" width="130px" height="50px">
                          Read More
                        </v-btn>
                      </v-card-actions>
                    </v-list-item-content>
                  </v-list-item>
                  </v-card>
                </v-col>
              </v-row>
              <!-- 스텝2 종료 -->
            </v-stepper-content>
            <v-stepper-content step="3">
              <!-- 슬라이드 스텝3 -->
              <v-row>
                <v-col cols="12" xs="12" sm="12" md="7" lg="7" xl="7">
                  <div class="cardImg">
                    <v-img src="/date.png" contain max-height="360"/>
                  </div>
                </v-col>
                <v-col cols="12" xs="12" sm="12" md="5" lg="5" xl="5">
                  <v-card class="mx-auto"  elevation="0">
                  <v-list-item>
                    <v-list-item-content>
                      <v-card-title class="fontStyleTitle">ABOUT US</v-card-title>
                      <v-card-text class="fontStyleH1">실시간 서버 공간 정보 검색</v-card-text>
                      <v-card-subtitle class="fontStyleH2">아래 세 가지 정보만을 입력 하여 서버공간의 <span>스케줄 및 최저가를 빠르게 검색</span> 할 수 있습니다.</v-card-subtitle>
                      <v-card-text>
                        <ul class="listStyle">
                          <li><v-icon dense>mdi-arrow-right-drop-circle-outline</v-icon> 이동하고자 하는 로컬 호스트</li>
                          <li><v-icon dense>mdi-arrow-right-drop-circle-outline</v-icon> 이동하고자 하는 로컬 호스트</li>
                          <li><v-icon dense>mdi-arrow-right-drop-circle-outline</v-icon> 이동하고자 하는 로컬 호스트</li>
                        </ul>
                      </v-card-text>
                      <v-card-actions>
                        <v-btn depressed color="accent" width="130px" height="50px">
                          Read More
                        </v-btn>
                      </v-card-actions>
                    </v-list-item-content>
                  </v-list-item>
                  </v-card>
                </v-col>
              </v-row>
              <!-- 스텝3 종료 -->
            </v-stepper-content>
            <v-stepper-content step="4">
              <!-- 슬라이드 스텝4 -->
              <v-row>
                <v-col cols="12" xs="12" sm="12" md="7" lg="7" xl="7">
                  <div class="cardImg">
                    <v-img src="/date.png" contain max-height="360"/>
                  </div>
                </v-col>
                <v-col cols="12" xs="12" sm="12" md="5" lg="5" xl="5">
                  <v-card class="mx-auto"  elevation="0">
                  <v-list-item>
                    <v-list-item-content>
                      <v-card-title class="fontStyleTitle">ABOUT US</v-card-title>
                      <v-card-text class="fontStyleH1">실시간 서버 공간 정보 검색</v-card-text>
                      <v-card-subtitle class="fontStyleH2">아래 세 가지 정보만을 입력 하여 서버공간의 <span>스케줄 및 최저가를 빠르게 검색</span> 할 수 있습니다.</v-card-subtitle>
                      <v-card-text>
                        <ul class="listStyle">
                          <li><v-icon dense>mdi-arrow-right-drop-circle-outline</v-icon> 이동하고자 하는 로컬 호스트</li>
                          <li><v-icon dense>mdi-arrow-right-drop-circle-outline</v-icon> 이동하고자 하는 로컬 호스트</li>
                          <li><v-icon dense>mdi-arrow-right-drop-circle-outline</v-icon> 이동하고자 하는 로컬 호스트</li>
                        </ul>
                      </v-card-text>
                      <v-card-actions>
                        <v-btn depressed color="accent" width="130px" height="50px">
                          Read More
                        </v-btn>
                      </v-card-actions>
                    </v-list-item-content>
                  </v-list-item>
                  </v-card>
                </v-col>
              </v-row>
              <!-- 스텝4 종료 -->
            </v-stepper-content>
        </v-stepper-items>
    </v-stepper>
  </div>
</template>

<script>
export default {
  name: 'AboutSlid',
  data: () => ({

  }),
}
</script>

<style scoped>
  .v-stepper__header{box-shadow:none;}
  .theme--light.v-stepper .v-stepper__step--editable:hover{background: none;}
  .v-stepper__step--active::after{content: ' '; height: 0; width: 0; position: absolute; bottom: -5px; border: 10px solid transparent; border-bottom-width: 0; border-top-color: #ddd; left: 77px;}
  .aboutTitle {text-align: center; padding: 80px 0 40px;}
  .aboutTitle p:first-child {font-size: 1.625rem; font-weight: 600;}
  .aboutTitle p:last-child {line-height: 30px}
  .aboutTitle span {color: #72c09f;}
  .cardImg{border: 1px solid #ddd; padding: 30px; max-height: 416px;}
  .fontStyleTitle{color: #72c09f; font-size: 0.938rem;}
  .fontStyleTitle::after{content: ' '; width: 30px; height: 2px; top: 33px; position: absolute; left: 114px; background: #72c09f;}
  .fontStyleTitle::before{content: ' '; width: 50px; height: 2px; top: 38px; position: absolute; left: 114px; background: #72c09f;}
  .fontStyleH1 {font-size: 1.688rem; font-weight: 600; letter-spacing: -1px;}
  .fontStyleH2 {font-size: 1.125rem; line-height: 30px; padding-top: 5px;}
  .fontStyleH2 span {font-weight: 600;}
  .listStyle {padding: 0; margin-top: 10px;}
  .listStyle li {list-style: none; line-height: 30px; font-size: 0.938rem;}
  .listStyle li i {color: #72c09f; margin-right: 2px;}
  .v-stepper__items{margin-top: 10px;}
  .v-card__actions{padding: 16px;}
  .v-application .accent{background-color: #72c09f !important; border-color: #72c09f !important;}
</style>
