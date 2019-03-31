<template>
  <div>
    <keep-alive>
        <component v-bind:is="component"></component>
    </keep-alive>
    <button v-on:click="component = 'form-one'">Show Form One</button>
    <button v-on:click="component = 'form-two'">Show Form Two</button>
  </div>
</template>

<script>


//Forms
import FormOne from './components/FormOne.vue'
import FormTwo from './components/FormTwo.vue'

export default {
  name: 'app',
  components: {
    'form-one': FormOne,
    'form-two': FormTwo
  },
  data(){
      return {
        component: 'form-two'
     }
  },
  methods: {

  }
}
</script>

<style scoped>

</style>
