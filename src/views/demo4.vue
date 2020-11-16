<template>
  <div id="demo4">
<h1>Data</h1>
<button @click="count++; isLogged = true;">count++</button>
<span>{{count}}</span>
<div>{{message}}</div>
<div>isLogged</div>
<input type="text" placeholder="Enter a massage" v-model="message"/>
<h2 v-if="isLogged">Yahoo</h2>
  </div>
</template>

<script>
export default {
name:'demo4',
mounted(){
  this.message="Welcome to tcvp";
},
data(){
  return {
    count:0,
    message:'',
    isLogged:false,

  };
},
};
</script>

<style>

</style>