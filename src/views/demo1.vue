<template>
  <div id="demo1">
       <test />
      <h1>v-model</h1>
      <input v-model="message" type="text" placeholder="Enter your message">
      <div>{{message}}</div>
      <button @click="message=''">Reset</button>
     
  </div>
</template>

<script>
import test from '../components/Test'
export default {
name:'demo1',
components:{
test
},
data(){
    return{
        message:""
    }
},
}
</script>

<style>

</style>