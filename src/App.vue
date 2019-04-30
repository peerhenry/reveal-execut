<template lang="pug">
  #app
    .reveal
      .slides
        Title
        Slide2(:monthCount="6")
        Slide2(:monthCount="2")
        section(data-transition="fade")
          section
            img(src="./assets/01_overview_1.png")
          section
            img(src="./assets/time/time1.png")
          section
            img(src="./assets/time/time2.png")
          section
            img(src="./assets/time/time3.png")
        section(data-transition="fade")
          img(src="./assets/02_overview_2.png")
        section(data-transition="fade")
          img(src="./assets/03_tech.png")
        section(data-transition="fade")
          img(src="./assets/04_devs.png")
        section
          video(controls width="156" height="544")
            source(src="./assets/ex/001.mp4" type="video/mp4")
        section
          img(src="./assets/ex/870_printer.png")
        section
          p https://github.com/infi-nl/Space-Invaders
</template>

<script>
import Reveal from 'reveal.js/js/reveal'

export default {
  name: 'app',
  components: {
    // HelloWorld
  },
  mounted() {
    Reveal.initialize()
  },
}
</script>

<style lang="scss">
@import '~reveal.js/css/reveal.css';
@import '~reveal.js/css/theme/black.css';

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* margin-top: 60px; */
  height: 100vh;
}

.wyte {
  background-color: white;
}
</style>
