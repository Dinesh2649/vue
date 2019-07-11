<template>
  <div>
    <input type="text" v-on:input="changeTitle">
    <h1>{{title}}</h1>
    
  </div>
</template>

<script>
export default {
  name: "sample2",
  data(){
  return{
       title:"reddy"
   }
  },
  methods:{
   changeTitle: function(event){
     this.title=event.target.value;
   }
  }
}


</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1{
  color:red;
  background-color:black;
}

</style>
