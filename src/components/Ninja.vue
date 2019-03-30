<template>
    <div>
        <h2>{{ title }}</h2>
        <ul>
            <li v-for="ninja in ninjas">{{ ninja }}</li>
        </ul>
    </div>
</template>

<script>
export default {
  name: 'Ninja',
   props: {
    title: String
   }, 
  data(){
      return {
       ninjas:["Francis", "Juni", "Tino", "Jeremiah"]
     }
  }
  
}
</script>
<style scoped>
h2 {
  color:green;
}

</style>