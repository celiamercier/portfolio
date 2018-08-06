<template>
  <b-container fluid>
    <nav class="root-nav">
      <ul class="main-nav">
        <li class="nav-item">
          <a href="#">Sketch</a>
          <div class="nav-item-decoration"></div>
        </li>
        <li class="nav-item">
          <a href="#">Animation</a>
          <div class="nav-item-decoration"></div>
        </li>
        <li class="nav-item">
          <a href="#">About</a>
          <div class="nav-item-decoration"></div>
        </li>
      </ul>
    </nav>
  </b-container>
</template>

<script>
  export default {
    name: 'menu-component'
  }
</script>

<style>
  .root-nav {
    text-align: center;
  }

  .main-nav {
    display: inline-block;
    padding-left: 0px;
    margin-bottom: 0px;
  }

  .nav-item {
    display: inline-block;
    margin-left: 30px;
  }
  .nav-item:first-of-type {
    margin-left: 0px;
  }

  .nav-item a {
    color: #C1B4A7;
  }
  .nav-item a:hover {
    color: #D6CBC0;
    text-decoration: none;
  }

  .nav-item-decoration {
    background-color: white;
    width: auto;
    height: 3px;
  }

  .nav-item a:hover + .nav-item-decoration {
    background-color: #D6CBC0;
    width: auto;
    height: 3px;
  }
</style>