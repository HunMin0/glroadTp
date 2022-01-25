<template>
<div class="at" v-show="visible">

    <v-app-bar app color="white" flat inverted-scroll >
      <div id="cloneLogo"><NuxtLogo2 /></div>
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
      <v-navigation-drawer
        width="50%"
        v-model="drawer"
        absolute
        temporary
        right
        style="position:fixed"
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

</template>

<script>
 export default {
    data: () => ({
      visible: false,
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
#cloneLogo {width: 300px; margin-left: 50px;}
.theme--light.v-tabs .v-tab:hover::before {opacity: 0;}
.theme--light.v-tabs .v-tab--active:focus::before {opacity: 0;}
.v-tab:hover  {color: #333 !important;}
.v-tab:before{display: none;}

#nav {height: 48px; text-align: right; width: 100%;}
.navLogo {margin-bottom: 10px;}
.v-list-item__title {text-align: left;font-size: 1rem;}

.at header{animation: wobble 0.5s; border-bottom: 1px solid #ededed!important;}
@keyframes wobble {
  0% { opacity:0; transform: translateY(-50px); }
  100% { opacity:1; transform: translateY(0px); }
}
</style>
