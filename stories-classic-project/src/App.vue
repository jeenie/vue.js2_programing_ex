<template>
  <div id="app">
    <img src="./assets/logo.png">
    <!--<hello></hello>-->
    <!--<login></login>-->
    <!--<register></register>-->
    <stories :stories="stories"></stories>
  </div>
</template>

<script>
import Login from './components/Login.vue'
import Hello from './components/Hello.vue'
import Register from './components/Register.vue'
import Stories from './components/Stories.vue'


export default {
  name: 'app',
  components: {
    Hello,
    Login,
    Register,
    Stories
  },
  data () {
    return {
      stories: [
        {
          plot: 'Mr horse is amazing.',
          writer: 'Mr.Weeb1',
          upvotes: 28,
          voted: false
        },
        {
          plot: 'Narwhals invented Shish Kebab.',
          writer: 'Mr.Weeb1',
          upvotes: 8,
          voted: false
        },
        {
          plot: 'The dark side of the Force is stronger.',
          writer: 'Darth Vader',
          upvotes: 52,
          voted: false
        },
        {
          plot: 'One does not simply walk into Mordo',
          writer: 'Boromir',
          upvotes: 74,
          voted: false
        }
      ]
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
