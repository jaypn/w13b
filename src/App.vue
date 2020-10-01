<template>
  <div id="app">
    <img alt="tweet logo" src="https://i.pinimg.com/originals/10/47/46/104746f957d0817fc76a4d871bcc5567.jpg">
    <tweet-page></tweet-page>
  </div>
</template>

<script>
import tweetPage from "./components/tweet.vue"

export default {
  name: 'App',
  components: {
    tweetPage,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
