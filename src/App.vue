<template>
  <div>
    <Addition />
    -----------------------------
    <Subtraction />
  </div>
</template>

<script lang="js">
import Addition from './components/Addition'
import Subtraction from './components/Subtraction'
 export default {
   name:"app",
   components:{
     Addition,
     Subtraction
   }
 }
</script>

<style>
 button {
   width: 60px;
   height: 25px;
 }
</style>