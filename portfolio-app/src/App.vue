<template>
  <b-container>
    <header-component/>
    <content-component v-bind:pictures="pictures"/>
  </b-container>
</template>

<script>
  import headerComponent from './components/header/Header.vue';
  import contentComponent from './components/content/Content.vue';

  export default {
    name: 'app',
    components: {
      headerComponent,
      contentComponent
    },
    data: function() {
      return {
        pictures: [
          {
            id: 0,
            title: "One Piece",
            desc: "Monkey D. Luffy as a girl",
            src: "http://www.quartier-japon.fr/sites/default/files/styles/image_detail_atelier/public/monkey_d._luffy_girl_03122015_0.jpg?itok=r5DDYh0k"
          },
          {
            id: 1,
            title: "Unknown",
            desc: "A manga that is does not know",
            src: "https://static.actu.fr/uploads/2018/02/radiant-1000x600-854x512.png"
          },
          {
            id: 2,
            title: "Bakemonogatari",
            desc: "Dangerous Senjougahara",
            src: "https://i2.wp.com/www.animeland.fr/wp-content/uploads/2018/03/ohgreat-2.jpg"
          },
          {
            id: 3,
            title: "Nichijou",
            desc: "Nichijou",
            src: "https://myanimelist.cdn-dena.com/images/anime/3/75617.jpg"
          },
          {
            id: 4,
            title: "Nichijou",
            desc: "Nichijou",
            src: "http://img.neko-san.fr/img/anime/535670dd0b0a6.jpg"
          },
          {
            id: 5,
            title: "Nichijou",
            desc: "Nichijou",
            src: "http://behind-the.nihonreview.com/wordpress/wp-content/uploads/2011/05/HorribleSubs-Nichijou-05-480p.mkv_snapshot_00.37_2011.05.02_20.17.29.jpg"
          }
        ]
      }
    }
  }
</script>

<style>
</style>
