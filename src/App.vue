<template>
  <v-app>
   <v-content>
     <v-router-view>
       <Login></Login>
       <Footer></Footer>
     </v-router-view>
   </v-content>
  </v-app>
</template>

<script>

import Login from './components/Login.vue';
import Footer from './components/Footer.vue'
export default {

  name: 'home',
  components:{
   Login,
  Footer
  },

  data: () => ({
    //
  }),
};
</script>
