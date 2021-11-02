<template>
  <div>
    <h3>当前最新的count值为：{{this.$store.state.count}}</h3>
    <button @click="add1"> +1 </button>
    <button @click="add2"> +N </button>

  </div>
</template>

<script lang="js">
export default {
  name: "addition",
  methods:{
    add1(){
      this.$store.commit('add');
    },
    add2(){
      this.$store.commit('addN',10);
    }
  }
}
</script>
