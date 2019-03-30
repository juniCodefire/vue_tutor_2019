<template>
  <!-- <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div> -->
  <div id="app">
    <app-header v-bind:title="title" v-on:changeTitle="updateTitle($event)"></app-header>
    <app-junininjas v-bind:ninjas="ninjas"></app-junininjas>
    <app-footer v-bind:copyright="copyright" v-bind:title="title"></app-footer>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

// export default {
//   name: 'app',
//   components: {
//     HelloWorld
//   }
// }
////////////////////////////////////////////////
// import FirstPage from './components/FirstPage.vue'
// import Ninja from './components/Ninja.vue'

////////////////////////////////////////////////
import Header from './components/Header.vue'
import JuniNinjas from './components/JuniNinjas.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'app',
  components: {
    'app-header': Header,
    'app-junininjas': JuniNinjas,
    'app-footer': Footer
  },
  data(){
      return {
       ninjas: [
           {name: 'Juni', speciality: "Magic Ninja", show: false},
           {name: 'Jeremiah', speciality: "Laravel", show: false},
           {name: 'Francis', speciality: "Lumen", show: false},
           {name: 'Tino', speciality: "Node.js", show: false},
           {name: 'Terry', speciality: "Vue Badass", show: false},
           {name: 'Freddy', speciality: "Andriod Guru", show: false}
       ],

       title: "Juni Ninja",
       copyright: "Copyright 2019"
     }
  },
  methods: {
    updateTitle: function (updatedTitle) {
      this.title = updatedTitle
    }
  }
}
</script>

<style scoped>

/* #app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
} */
</style>
