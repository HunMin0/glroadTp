<template>
  <div class="at" v-show="visible">
    <v-app-bar app color="white" flat inverted-scroll >
      <div id="cloneLogo"><Logo2 /></div>
      <v-tabs centered class="ml-n9 openMenu" color="#111 darken-1" background-color="transparent">
      <v-tab v-bind:title="link.tab" class="resize"
        v-for="link in links"
        :key="link.tab"
        :to="link.href"
        :ripple="false"
        >
        {{ link.tab }}
        </v-tab>
    </v-tabs>
    <div class="quickNav">
      <v-app-bar-nav-icon @click="drawer = true" color="#333" large></v-app-bar-nav-icon>
    </div>
    </v-app-bar>
    <v-navigation-drawer width="50%" v-model="drawer" absolute temporary right style="position:fixed; z-index:9999">
      <v-list flat>
        <v-list-item-group v-model="group" active-class="grey lighten-5">
          <v-list-item class="navLogo"><Logo2 /></v-list-item>
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
</template>

<script>
 export default {
    data: () => ({
      visible: false,
      drawer: false,
      group: null,
      absolute: true,
      links: [
        {tab: 'HOME', href: '/', icon:'mdi-inbox'},
        {tab: 'ABOUT US', href: '/temple', icon:'mdi-star'},
        {tab: 'BUSINESS', href: '/#', icon:'mdi-send'},
        {tab: 'PRODUCT', href: '/#', icon:'mdi-send'},
        {tab: 'SUPPORT', href: '/#', icon:'mdi-send'},
      ],
    }),
    methods: {
      scrollTop: function () {
        this.intervalId = setInterval(() => {
          if (window.pageYOffset === 0) {
            clearInterval(this.intervalId)
          }
          window.scroll(0, window.pageYOffset - 50)
        }, 20)
      },
      scrollListener: function (e) {
        this.visible = window.scrollY > 150
      }
    },
    mounted: function () {
      window.addEventListener('scroll', this.scrollListener)
    },
    beforeDestroy: function () {
      window.removeEventListener('scroll', this.scrollListener)
    }
  }

</script>

<style scoped>
#cloneLogo {width: 30%; margin-left: 350px;}
.theme--light.v-tabs .v-tab:hover::before {opacity: 0;}
.theme--light.v-tabs .v-tab--active:focus::before {opacity: 0;}
.v-tab:hover  {color: #333 !important;}
.v-tab:before{display: none;}
#nav {height: 48px; text-align: right; width: 100%;}
.navLogo {margin-bottom: 10px;}
.v-list-item__title {text-align: left;font-size: 1rem;}
.at header{animation: wobble 0.5s; border-bottom: 1px solid #ededed!important; z-index: 9999;}
@keyframes wobble {
  0% { opacity:0; transform: translateY(-50px); }
  100% { opacity:1; transform: translateY(0px); }
}
@media (max-width: 2000px){
    #cloneLogo {margin-left: 50px;}
  }
  @media (max-width: 960px){
    #cloneLogo {margin-left: 0;}
  }
</style>
