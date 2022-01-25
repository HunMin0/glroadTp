<template>

<v-container fluid class="ma-0 pa-0" fill-height>
  <v-row>
    <v-col>

      <Menu ref="menu" />
      <!-- 메인비쥬얼 -->
      <v-carousel
          fullscreen
          height="calc(100vh - 0px)"
          hide-delimiter-background
          show-arrows-on-hover
          hide-delimiters
          >

        <v-carousel-item
          v-for="(item,i) in items"
          :key="i"
          :src="item.src"
        >
        <v-row>
          <v-col>
            <!-- 오버레이영역 -->
            <div class="overlayMam">
              <!-- 비쥬얼 텍스트 -->
              <v-row justify="center" align="center" class="setHeight">
                <v-spacer/>
                  <v-col cols="10" xs="10" sm="8" md="8" lg="10" xl="l0">

                    <div class="textTitle animate__animated animate__fadeInRight fadeInRight">
                      <p class="">NUXT ANIMEJS</p>
                      <p class="slidTitle" v-text="item.fristText"></p>
                      <p class="slidSub" v-text="item.lastText"></p>
                    </div>
                    <div class="visualMore animate__animated animate__fadeIn animate__delay-1s" title="더보기"><router-link :to="item.link">더보기</router-link></div>

                  </v-col>
                <v-spacer/>
              </v-row>
              <v-row class="btArr animate__animated animate__fadeIn animate__delay-2s">
                <v-col>
                  <div class="bottomArr" title="이동">
                      <div class="s">
                        <v-btn
                          class="align-self-end mt-15"
                          color="#fff"
                          fab
                          outlined
                          @click="$vuetify.goTo('#about')"
                        >
                        <v-icon>mdi-chevron-down</v-icon>
                        </v-btn>
                      </div>
                    </div>
                </v-col>
              </v-row>
            </div>
           <v-overlay :value="overlay" class="overlayStyle" />
            <!-- 오버레이영역 종료-->
          </v-col>
        </v-row>
        </v-carousel-item>
      </v-carousel>

    </v-col>
  </v-row>
</v-container>

</template>

<script>


export default {
  name: 'Visual',

  data: () => ({
    items: [
      {
        src: '/bg02.jpg',
        fristText: '간편하고 빠른 VUE서비스 NUXT와 함께',
        lastText: '더 낮은 곳을 향해 세상의 가치를 이동합니다.',
        link: '/'
      },
      {
        src: '/bg01.jpg',
        fristText: '간편하고 빠른 VUE서비스 NUXT와 함께',
        lastText: '더 낮은 곳을 향해 세상의 가치를 이동합니다.',
        link: '/'
      },
    ],
    }),
}
</script>

<style scope>
.theme--light.v-tabs .v-tab:hover::before {opacity: 0;}
.theme--light.v-tabs .v-tab--active:focus::before {opacity: 0;}

.overlayMam {width: auto; height: 100vh; position: relative; z-index: 999;}
.overlayStyle{position: absolute; z-index: 99;}

.textTitle {color: #fff;}
.slidTitle {font-size: 3rem;}
.slidSub{font-size: 1.2rem;}
.visualMore {margin: 40px 0 0 0;}
.visualMore a {padding: 14px 40px; border: 1px solid #a5a5a5; text-decoration: none; color: #ddd !important;}
.visualMore a:hover {background: rgb(255 255 255 / 5%);}
.btArr {position: absolute; bottom: 40px; width: 100%;}
.bottomArr {text-align: center;}

@keyframes fadeInRight {
  from {
    opacity: 0;
    transform: translateX(300px);
  }
  to {
    opacity: 1;
  }
}
</style>
