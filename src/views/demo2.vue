<template>
  <div id="demo2">
    <h1>demo2 EvenMethods</h1>
    <button v-on:click="clickMe">clickMe</button>
    <button v-on:click="clickMe2('Welcome to vueJS')">clickMe2</button>
    <button @click="clickMe2('Welcome to VangVieng')">clickMe3</button>
    <h3>{{getTimestamp()}}</h3>
  </div>
</template>

<script>
export default {
name:'demo2',
mounted(){
  this.initial()
  
},
methods:{
  initial(){
  console.log("Initiallization")
  },
  clickMe(){
    alert('Hi')
  },
  clickMe2(message){
    alert(message)
  },
  getTimestamp(){
      return Date()
    }

  }
}

</script>

<style>

</style>