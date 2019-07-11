<template>
  <div class="hello" >
    <h1>{{ name }}</h1>
    <table v-if="isVisible">
         <tr>
             <th>name</th>
             <th>age</th>
         </tr>
         <tr v-for="Item in person">
              <td>{{Item.name}}</td>
              <td>{{Item.age}}</td>
         </tr>

    </table>
    <h4 v-if="isVisible">dinu</h4>
    <h5 v-else="!isVisible">bindu</h5>
    <a href="link">google</a>
   
    <button @click="abc">submit</button>
    <h2 :style="{ color:'pink'}">bhaskar reddy</h2>
    <h3 :style="js">sujatha</h3>
    <h1>sdfghjklkjhgzxghj</h1>
   </div>
</template>

<script>
export default {
  name: 'sample',
  data(){
  return{  
  person:[{name:"bhaskar",age:23},{name: "koti",age: 27},{name: "mahesh",age: 28}],
  isVisible:true,
   js :{
      color:'pink',
      background:'green'
    },
    link: 'http://google.com'
   }
  },
  methods:{
   abc: function(){
   this.isVisible=!this.isVisible
   console.log(this.isVisible)
   }
   
  }
}


</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1{
  color:blue;
  background-color:red
}
table,th,td{
  border:1px solid red;
  border-collapse:collapse;
  background-color:yellow;
}
</style>
