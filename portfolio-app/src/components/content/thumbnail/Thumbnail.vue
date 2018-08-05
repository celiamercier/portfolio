<template>
  <b-img-lazy thumbnail fluid :src="img.src"/>
</template>

<script>
  export default {
    name: 'thumbnail-component',
    props: [ 'img' ]
  }
</script>

<style></style>