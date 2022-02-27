<template>
    <v-app-bar
      style="padding: 0px 90px"
      app
      color="white"
      light
      elevation="6"
      elevate-on-scroll
    >

    <v-toolbar-title>
      Software Hunt
    </v-toolbar-title>
  <v-spacer></v-spacer>
    <v-list class="d-flex align-center">
    <v-list-item link v-for="(menu,index) in menus" :key="index" :to="menu.route">
      <v-list-item-title>{{menu.title}}</v-list-item-title>
    </v-list-item>
    </v-list>
  <v-btn text>
    <v-icon>mdi-magnify</v-icon>
  </v-btn>
  <v-btn outlined color="success">
    Get Started
  </v-btn>
    </v-app-bar>
</template>

<script>
export default {
    name: 'Header',
    data() {
    return {
      menus: [
        {title:'Home', route:'home'},
        {title:'About Us', route:'about-us'},
        {title:'Portfolio', route:'portfolio'},
        {title:'Project', route:'project'},
        {title:'Gallery', route:'gallery'},
        {title:'Contact', route:'contact'},
        
      ]
    }
  },
}
</script>

<style scoped>
.v-toolbar__title{
    font-size: 32px;
    color: #4caf50;
    font-weight: 700;
    font-family: cursive ;
    }
</style>