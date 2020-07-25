<template>
  <div id="app">
    <section class="left-pane">
      <div class="portrait" />
      <h1>Hi, I'm Jason.</h1>
      <h2>I'm a Software Engineer && UI/UX/U∞ Designer from Austin, TX.</h2>
      <p>Over a decade in the web/software development field. I like to work where Art + Sciene meet and where data gets involved. This is where I showcase some of my projects that I think are fun.</p>
    </section>
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <main class="portfolio-stage">
      <section class="portfolio-topic apps">
        <h3>Here's some stuff I built using Vue.js, Ember.js and React:</h3>
        <ul>
          <li><a href="austin-fc-kit-creator.netlify.app" title="">Austin FC Kit Creator (Vue.js + SVGs)</a></li>
          <li><a href="https://circler.netlify.com/" title="">The Circler - SVG-Driven Generative Art (React + SVGs)</a></li>
          <li><a href="https://background-playground.netlify.com/" title="">Background Playground (Ember.js)</a></li>
          <li><a href="Subreddit Surfer (React + Reddit API)" title="">Subreddit Surfer (React + Reddit API)</a></li>
          <li><a href="SVG Playground - Play around with configuring SVGs for different aesthetics (Ember.js)" title="">SVG Playground - Play around with configuring SVGs for different aesthetics (Ember.js)</a></li>
          <li><a href="https://qol-report.netlify.com/" title="">Quality of Life Report (Vue.js + Teleport API)</a></li>
          <li><a href="https://color-with-a-you.netlify.com/" title="">Colour with a You (Vue.js + chroma.js)</a></li>
          <li><a href="https://leaflet-vue.netlify.com/" title="">My Career Path (Vue.js + Leaflet)</a></li>
          <li><a href="https://drinkingtheink.github.io/dnb_notifications" title="">Interface Notification System</a></li>
          <li><a href="https://drinkingtheink.github.io/dogtastic" title="">Dogtastic! Name and claim the dogs of your choice</a></li>
        </ul>
      </section>
    </main>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  data() {
    return {

    }
  }
};
</script>

<style lang="scss">
@import './styles/palette';

body,
html {
  background-color: rgba(black, 0.4);
  padding: 0;
  margin: 0;
}

#app {
  display: flex;
  justify-content: space-between;
}

$leftPaneWidth: 20vw;
$mainPaneWidth: 100 - $leftPaneWidth - 4;

.left-pane,
main {
  background-color: rgba(black, 0.4);
  padding: .5em;
  height: 100vh;
}

.left-pane {
  width: $leftPaneWidth;
}

$portraitDim: 10em;

.portrait {
  margin: 0 auto;
  height: $portraitDim;
  width: $portraitDim;
  background: url(https://drinkingtheink.github.io/img/jmh_WEB.jpg) no-repeat center;
  background-size: contain;
  border-radius: 50%;
  border: 3px solid #1A535C;
}

.portfolio-stage {
  width: $mainPaneWidth;
}
</style>
