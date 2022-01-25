<template>
  <v-row>
    <v-col>
      <v-responsive>
       <v-carousel
          fullscreen
          cycle
          height="calc(100vh - 100px)"
          hide-delimiter-background
          show-arrows-on-hover
          hide-delimiters
        >

        <template v-slot:prev="{ on, attrs }">
        <v-btn
          color="success"
          v-bind="attrs"
          v-on="on"
        >PREV</v-btn>
      </template>
      <template v-slot:next="{ on, attrs }">
        <v-btn
          color="info"
          v-bind="attrs"
          v-on="on"
        >NEXT</v-btn>
      </template>
          <v-carousel-item>
            <v-sheet
              height="100%"
            >
              <v-row
                class="fill-height mx-auto"
                align="center"
                justify="center"
                style="background:url(/bg.jpg) center/cover no-repeat"
                max-width="1280"
              >
                <v-card  color="transparent">
                  <p class="text-h3 white--text font-weight-bold text-center">안전하고 편리한 영상 서비스</p>
                  <p class="text-subtitle-1 white--text font-weight-thin text-center">안전한 비즈니스 회의를 위한 WebMeeting 서비스를<br>누구나 간편하게 사용할 수 있습니다.</p>
                </v-card>
              </v-row>
            </v-sheet>
          </v-carousel-item>
          <v-carousel-item>
            <v-sheet
              height="100%"
            >
              <v-row
                class="fill-height mx-auto"
                align="center"
                justify="center"
                style="background:url(/bg.jpg) center/cover no-repeat"
                max-width="1280"
              >
                <v-card  color="transparent">
                  <p class="text-h3 white--text font-weight-bold text-center">안전하고 편리한 영상 서비스</p>
                  <p class="text-subtitle-1 white--text font-weight-thin text-center">안전한 비즈니스 회의를 위한 WebMeeting 서비스를<br>누구나 간편하게 사용할 수 있습니다.</p>
                </v-card>
              </v-row>
            </v-sheet>
          </v-carousel-item>
          <v-carousel-item>
            <v-sheet
              height="100%"
            >
              <v-row
                class="fill-height mx-auto"
                align="center"
                justify="center"
                style="background:url(/bg.jpg) center/cover no-repeat"
                max-width="1280"
              >
                <v-card  color="transparent">
                  <p class="text-h3 white--text font-weight-bold text-center">안전하고 편리한 영상 서비스</p>
                  <p class="text-subtitle-1 white--text font-weight-thin text-center">안전한 비즈니스 회의를 위한 WebMeeting 서비스를<br>누구나 간편하게 사용할 수 있습니다.</p>
                </v-card>
              </v-row>
            </v-sheet>
          </v-carousel-item>
        </v-carousel>
      </v-responsive>
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: 'IndexPage',

}
</script>
