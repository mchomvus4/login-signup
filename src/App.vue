<template>
  <v-app>
   <v-main>
     <v-router-view>
       <Login/>
       <Footer/>
     </v-router-view>
   </v-main>
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
