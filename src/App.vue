<template>
  <div id="app">
    <HelloWorld />
<ul>
    <li><router-link to="/">Home</router-link></li>
    <li><router-link to="/demo1">demo1</router-link></li>
    <li><router-link to="/demo2">demo2</router-link></li>
    <li><router-link to="/demo3">demo3</router-link></li>
    <li><router-link to="/demo4">demo4</router-link></li>
</ul>
<router-view></router-view>
<test />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import test from './components/Test'

export default {
name:'app',
components:{
  HelloWorld,
  test
}
}
</script>

<style>
ul{
    margin: 0;
    padding: 0;
}
li{
    display: inline;
    margin: 8px;
}
</style>