<template>
  <div>
    <header_component></header_component>
    <content_component></content_component>
  </div>
</template>

<script>
  import header_component from './components/header/Header.vue';
  import content_component from './components/content/Content.vue';

  export default {
    name: 'app',
    components: {
      header_component,
      content_component
    }
  }
</script>

<style>
</style>
