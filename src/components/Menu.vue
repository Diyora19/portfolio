<template>
    <div>
  
    <v-app-bar
      class="bar px-5"
      flat
      dense
      app

    >

      <v-toolbar-title class="link grey--text">Portfolio</v-toolbar-title>

      <v-spacer></v-spacer>
      
    
    <router-link to="/" class="link grey--text">Home</router-link>
    <router-link to="/aboutme" class="link grey--text">About Me</router-link>
    <router-link to="/portfolio" class="link grey--text">Portfolio</router-link>
      
    </v-app-bar>

    </div>
</template>

<script>
export default {
    name: 'Menu'
}
</script>

<style>
.link{
    text-decoration: none;
    padding: 0 10px;
    font-weight: 500;
    font-size: 18px;
}
.bar{
    background: rgba(240, 238, 238, 0.5)!important;;
}

</style>