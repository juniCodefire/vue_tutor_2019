<template>
    <div>
        <h2>{{ title }}</h2>
        <p>{{greeting()}}</p>
    </div>
</template>

<script>
export default {
  name: 'FisrtPage',
  props: {
    title: String
  },
  methods: {
     greeting: function () {
        return "Hey vue is cool!"
      }
  }
}
</script>
<style scoped>

h2 {
  color:orangered;
}
/* #app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
} */
</style>