<template>
  <v-app>

    <v-main class="main">
      <Menu />      
      <router-view/>
      <Footer class="footer"/>
    </v-main>
  </v-app>
</template>

<script>
import Footer from './components/Footer.vue';
import Menu from './components/Menu.vue';

export default {
  name: 'App',
  components: {Menu, Footer},

  data: () => ({
    //
  }),
};
</script>

<style>
.main{
  background: url('./assets/img/glass-card1.jpg');
  background-repeat: no-repeat;
  background-position: center;
  background-attachment: fixed;
  background-size: cover;

}

.footer{
  position: fixed;
  bottom: 0;
  text-align: center;
  width: 100%;
}


</style>
