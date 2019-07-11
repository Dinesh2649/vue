<template>
  <div>
  <p>{{sayhello()}}</p>
    <p><a :href=link>google</a></p>
    <button @click="increase">click me</button>
    <p>{{ counter }}</p>
    <button @click="changelink">click to change link</button>
    <a href="link">link</a>
    <div class="demo" :style="{background:'blue'}"></div>
    <div class="demo"></div>
    <div class="demo"></div>
    <h1>qwertyuiopasdfghjklzxcvbnm</h1>
    <h1> HARI NATH REDDY</h1>
  </div>
</template>

<script>
export default {
  
  data() {
  return {
     
      title:"hello world",
       link:"http://google.com",
       counter: 0,
       link:"http://facebook.com"

   }
  },
   created () {
       this.sayhello()
   },
  methods:{
   sayhello: function(){
    alert("jnhgfdcvgbgvfdc");
   },
   increase: function() {
       this.counter++;
   },
   changelink: function(){
   this.link = "http://gmail.com";
   }
}
}


</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.demo {
    width: 100px;
    height: 100px;
    background-color: gray;
    display: inline-block;
    margin: 10px;
}


</style>
