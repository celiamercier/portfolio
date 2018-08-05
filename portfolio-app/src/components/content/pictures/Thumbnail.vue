<template>
  <b-img-lazy v-b-modal.pictureModal thumbnail fluid :src="img.src"/>
</template>

<script>
  export default {
    name: 'thumbnail-component',
    props: [ 'img' ]
  }
</script>

<style></style>