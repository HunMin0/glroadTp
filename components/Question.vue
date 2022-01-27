<template>
  <div class="question">
    <div class="PromotionTitle">
      <h1>비즈니스<span>제휴문의</span></h1>
      <p>제휴 및 제안은 본 시스템을 통해 접수된 건에 한하여 정식으로 검토되며 제안 내용 및 관련자료는 제휴 검토 목적으로만 이용됩니다.</p>
    </div>
     <v-container fluid>
      <v-row align="center" justify="center">
        <v-col cols="10" xs="10" sm="10" md="8" lg="8" xl="6">
          <v-row>문의정보</v-row>
          <v-row>
            <v-col>
              <v-card>
              <v-card-title>이름</v-card-title>
             <v-card-text>
              <v-text-field filled rounded label="이름을 입력해주세요" color="#ddd"></v-text-field>
            </v-card-text>
 </v-card>
            </v-col>
            <v-col>
              <v-card-title>연락처</v-card-title>
               <v-card-text>
              <v-text-field filled rounded label="예) 010-1234-5678" color="#ddd"></v-text-field>
            </v-card-text>
            </v-col>
          </v-row>
        </v-col>
      </v-row>
     </v-container>

  </div>
</template>

<script>
export default {
  name: 'Question',
  data: () => ({
    items: [
      {

      },
    ],
  }),
}
</script>

<style scoped>
.question{min-height: 600px;}
@media (min-width: 605px){

}
@media (max-width: 960px){

}
</style>
