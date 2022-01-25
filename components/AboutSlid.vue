<template>
  <div class="aboutSlid">
    <div class="aboutTitle">
      <p>「누구나 쉽게 수출 할 수 있는 디지털 NUXT 플랫폼」</p>
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
                <v-card
                    class="ma-0 pa-0"
                    color="#ddd"
                    height="400px"
                    flat
                ><v-img src="images/about/about1.png"></v-img></v-card>
            </v-stepper-content>
            <v-stepper-content step="2">
                <v-card
                     class="ma-0 pa-0"
                    color="#ddd"
                    height="400px"
                    flat
                ><v-img src="images/about/about2.png"></v-img></v-card>
            </v-stepper-content>
            <v-stepper-content step="3">
                <v-card
                     class="ma-0 pa-0"
                    color="#ddd"
                    height="400px"
                    flat
                ><v-img src="images/about/about3.png"></v-img></v-card>
            </v-stepper-content>
            <v-stepper-content step="4">
                <v-card
                    class="ma-0 pa-0"
                    color="#ddd"
                    height="400px"
                    flat
                ><v-img src="images/about/about4.png"></v-img></v-card>
            </v-stepper-content>
        </v-stepper-items>
    </v-stepper>
  </div>
</template>

<script>
export default {
  name: 'AboutSlid',
}
</script>

<style scoped>
  .v-stepper__header{box-shadow:none;}
  .theme--light.v-stepper .v-stepper__step--editable:hover{background: none;}
  .v-stepper__step--active::after{content: ' '; height: 0; width: 0; position: absolute; bottom: -5px; border: 10px solid transparent; border-bottom-width: 0; border-top-color: #ddd; left: 77px;}
  .aboutTitle {text-align: center; padding: 60px 0 40px;}
  .aboutTitle p:first-child {font-size: 26px; font-weight: 600;}
  .aboutTitle p:last-child {line-height: 30px}

</style>
