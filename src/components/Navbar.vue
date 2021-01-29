<template>
   <nav>
      <v-navigation-drawer  v-model="drawer" dark app mini-variant class="pink accent-2">
          <v-list tile>
               <v-list-item class="mb-5" router to="/">
                  <v-list-item-action>
                     <v-icon >fas fa-window-restore</v-icon>
                  </v-list-item-action>
              </v-list-item>
              <v-list-item  class="mb-8">
                  <v-list-item-action>
                     <v-icon >far fa-clock</v-icon>
                  </v-list-item-action>
              </v-list-item>
              <v-list-item  class="mb-8">
                  <v-list-item-action>
                     <v-icon >fas fa-chart-line</v-icon>
                  </v-list-item-action>
              </v-list-item>
              <v-list-item  class="mb-8">
                  <v-list-item-action>
                     <v-icon >far fa-comment-alt</v-icon>
                  </v-list-item-action>
              </v-list-item>
              <v-list-item  >
                  <v-list-item-action>
                     <v-icon >fas fa-cog</v-icon>
                  </v-list-item-action>
              </v-list-item>
          </v-list>
      </v-navigation-drawer>
       <v-navigation-drawer  v-model="right" dark app  class="deep-orange accent-2"  fixed right>
           <v-layout column align-center>
               <v-flex class="mt-5"> 
                    <v-avatar size="100">
                            <img src="/img1.png" alt="">
                    </v-avatar>
                    <h4 class="white--text subheading mt-1 text-center">Julian Neal</h4>
                    <h6 class="white--text subheading mt-1 text-center">CEO.Almz Pvt.Ltd</h6>
               </v-flex>
          </v-layout>
           <p class="white--text subheading pl-3 mt-3">Rank of Company</p>
          <v-list rounded dense>
               <v-list-item  router to="/">
                  <v-list-item-action>
                     03
                  </v-list-item-action>
                  <v-list-item-content>
            <v-list-item-title >The Income</v-list-item-title>
                  </v-list-item-content>
              </v-list-item>
              <v-list-item  router to="/">
                  <v-list-item-action>
                     05
                  </v-list-item-action>
                  <v-list-item-content>
            <v-list-item-title >Human Resources</v-list-item-title>
                  </v-list-item-content>
              </v-list-item>
               <v-list-item  router to="/">
                  <v-list-item-action>
                     12
                  </v-list-item-action>
                  <v-list-item-content>
            <v-list-item-title >The Growth</v-list-item-title>
                  </v-list-item-content>
              </v-list-item>
          </v-list>
           <p class="white--text subheading pl-3 mt-3">Next Meeting Places</p>
           <v-timeline align-top dense fill-dot small dark>
                <v-timeline-item fill-dot small color="white" class="white--text">Morisseeberg</v-timeline-item>
                <v-timeline-item  fill-dot small color="white" class="white--text">East Mortonstad</v-timeline-item>
                <v-timeline-item  fill-dot small color="white" class="white--text">Andersonland</v-timeline-item>
            </v-timeline>
      </v-navigation-drawer>
   </nav>
</template>
<script>
export default {
   data: () => ({
      drawer: true,
      right: true,
      links :[
          {icon: 'fas fa-desktop', route: '/'},
          {icon: 'fas fa-shopping-cart',  route: '/shopping'},
          {icon: 'fas fa-city',  route: '/city'},
          {icon: 'fas fa-cog',  route: '/cog'}
      ]
     
    }),
    components: {

  },

   
}
</script>
<style scoped>
.border {
  border-left: 4px solid #0ba518;
}
</style>
