<template>
  <b-container fuild id="content">
    <b-row>
      <b-col>
        <thumbnail-component v-for="img in firstColumn" v-bind:key="img.id" v-bind:img="img"/>
      </b-col>
      <b-col>
        <thumbnail-component v-for="img in secondColumn" v-bind:key="img.id" v-bind:img="img"/>
      </b-col>
      <b-col>
        <thumbnail-component v-for="img in thirdColumn" v-bind:key="img.id" v-bind:img="img"/>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
  import thumbnailComponent from './thumbnail/Thumbnail.vue';

  export default {
    name: 'contentComponent',
    props:[ 'pictures' ],
    components: {
      thumbnailComponent
    },
    computed: {
      firstColumn: function () {
        let images = [];
        for (let i = 0; i < this.pictures.length; i +=3) {
          images.push(this.pictures[i]);
        }
        return images;
      },
      secondColumn: function () {
        let images = [];
        for (let i = 1; i < this.pictures.length; i +=3) {
          images.push(this.pictures[i]);
        }
        return images;
      },
      thirdColumn: function () {
        let images = [];
        for (let i = 2; i < this.pictures.length; i +=3) {
          images.push(this.pictures[i]);
        }
        return images;
      }
    }
  }
</script>

<style>
  #content {
    padding: 10px;
  }
</style>