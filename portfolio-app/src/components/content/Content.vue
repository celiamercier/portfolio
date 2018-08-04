<template>
  <div id="content" class="container-fluid">
    <div class="row">
      <div class="col-sm">
        <thumbnail_component></thumbnail_component>
      </div>
      <div class="col-sm">
        <thumbnail_component></thumbnail_component>
      </div>
      <div class="col-sm">
        <thumbnail_component></thumbnail_component>
      </div>
    </div>
  </div>
</template>

<script>
  import thumbnail_component from './thumbnail/Thumbnail.vue';

  export default {
    name: 'content_component',
    components: {
      thumbnail_component
    }
  }
</script>

<style>
  #content {
    border: solid 1px black;
  }
</style>