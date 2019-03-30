<template>
    <footer>
        <p>{{copyright}} {{title}}</p>
    </footer>
</template>

<script>
export default {
  name: 'Footer',
   props: {
       title: {
           type: String,
           required: true
       },
        copyright:{
            type: String,
            required: true
        }
   }, 
  data(){
      return {
       
     }
  }
  
}
</script>
<style scoped>
footer {
    background:#222;
    padding:6px;
}
p {
    color:lightgreen;
    text-align: center;
    font-size: 15px;
}

</style>