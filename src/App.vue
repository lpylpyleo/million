<template>
  <div id="app">
    <Card v-for="idol in idols" :title="idol.name" img="https://storage.matsurihi.me/mltd/card/033sih0114_0_b.png"
    text="nyan nyan" footer="add in fes" :key="idol.id"/>
  </div>
</template>

<script>
import Card from './components/Card.vue'
import idols from '../resources/idols'

export default {
  name: 'app',
  components: {
    Card: Card
  },
  data() {
    return {
      idols:idols
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
