<template>

<v-container fluid class="hot_line">


  <v-row><v-spacer/>
    <v-col cols="8"  xs="8" sm="8" md="2" lg="3" xl="3">
      <NuxtLogo />
    </v-col>
    <v-col cols="2"  xs="2" sm="2" md="9" lg="7" xl="7">
      <div id="nav">

        <div class="openMenu">
          <v-tabs dark centered class="ml-n9" color="#fff" background-color="transparent">
            <v-tab v-bind:title="link.tab" class="resize"
              v-for="link in links"
              :key="link.tab"
              :to="link.href"
              :ripple="false"
            >
            {{ link.tab }}
            </v-tab>
            <v-tabs-slider color="transparent" />
          </v-tabs>
        </div>

        <div class="quickNav">
          <v-app-bar-nav-icon @click="drawer = true" color="#fff" large ></v-app-bar-nav-icon>
          <v-navigation-drawer
            width="50%"
            v-model="drawer"
            absolute
            temporary
            right
          >
            <v-list flat>
              <v-list-item-group
                v-model="group"
                active-class="grey lighten-5"
              >
                <v-list-item class="navLogo"><NuxtLogo2 /></v-list-item>
                <v-list-item
                  v-for="link in links"
                  :key="link.tab"
                  :to="link.href"
                  style="height:60px"
                >
                  <v-list-item-icon>
                    <v-icon v-text="link.icon"/>
                  </v-list-item-icon>

                  <v-list-item-content>
                  <v-list-item-title v-text="link.tab"/>
                 </v-list-item-content>

                </v-list-item>

              </v-list-item-group>
            </v-list>
          </v-navigation-drawer>
        </div>

      </div>
    </v-col >
    <v-spacer/>

  </v-row>


</v-container>

</template>

<script>
 export default {
    data: () => ({
      drawer: false,
      group: null,
      absolute: true,
      links: [
        {tab: 'home', href: '/', icon:'mdi-inbox'},
        {tab: 'subpage1', href: '/temple', icon:'mdi-star'},
        {tab: 'subpage2', href: '/#', icon:'mdi-send'},
        {tab: 'subpage3', href: '/#', icon:'mdi-send'},
        {tab: 'subpage4', href: '/#', icon:'mdi-send'},
      ],
    }),
    methods: {
      closeNew () {
        if(this.drawer == true){
          document.getElementsByClassName("v-window__next")[0].style.display = "none";
        } else{
          document.getElementsByClassName("v-window__next")[0].style.display = "block";
        }
      },

    },

  }
</script>

<style scoped>
.theme--dark.v-tabs .v-tab--active:hover::before, .theme--dark.v-tabs .v-tab--active::before {opacity: 0;}
.theme--dark.v-tabs .v-tab:hover::before {opacity: 0;}
.v-tab {font-size: 0.930rem;}
.v-tab:hover  {color: #fff !important;}
.v-tab:before{display: none;}

#nav {height: 48px; text-align: right;}
.navLogo {margin-bottom: 10px;}
.v-list-item__title {text-align: left;font-size: 1rem;}
</style>
