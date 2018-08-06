<template>
  <b-container id="header">
    <h1>Yvanya</h1>
    <menu-component id="navigation"></menu-component>
  </b-container>
</template>

<script>
  import MenuComponent from "./menu/Menu.vue";

  export default {
    name: 'header-component',
    components: { MenuComponent }
  }
</script>

<style>
  @import url('https://fonts.googleapis.com/css?family=Gloria+Hallelujah');

  #header {
    padding-top: 50px;
    padding-bottom: 30px;
  }

  #header h1 {
    color: #C1B4A7;
    font-family: 'Gloria Hallelujah', cursive;
    text-align: center;
    font-size: 400%;
  }

  #navigation {
    margin-top: 60px;
  }
</style>