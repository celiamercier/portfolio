<template>
  <b-container fuild id="content">
    <b-row>
      <b-col class="p-1">
        <thumbnail-component v-for="img in computeColumn(0)"
                             v-bind:key="img.id"
                             v-bind:img="img"/>
      </b-col>
      <b-col class="p-1">
        <thumbnail-component v-for="img in computeColumn(1)"
                             v-bind:key="img.id"
                             v-bind:img="img"/>
      </b-col>
      <b-col class="p-1">
        <thumbnail-component v-for="img in computeColumn(2)"
                             v-bind:key="img.id"
                             v-bind:img="img"/>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
  import thumbnailComponent from './pictures/Thumbnail.vue';

  export default {
    name: 'contentComponent',
    props:[ 'pictures' ],
    components: {
      thumbnailComponent
    },
    methods: {
      computeColumn: function (offset) {
        let images = [];
        for (let i = offset; i < this.pictures.length; i +=3) {
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