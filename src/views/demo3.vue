<template>
  <div id="demo3">
    <h1>{{message}}</h1>
    <h2>{{count}}</h2>
    <button @click="onClickAdd">Add</button>
  </div>
</template>

<script>
export default {
name:'demo3',
data(){
  return {
    message:'Data',
    count: 0
  }
},
methods: {
  onClickAdd(){
    this.count=this.count+1
  }
}
}
</script>

<style>

</style>