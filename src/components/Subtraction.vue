<template>
  <div>
    <h3>当前最新的count值为：{{count}}</h3>
    <button @click="sub1"> -1 </button>
    <button @click="sub2"> -N </button>
  </div>
</template>

<script lang="js">
import {mapState,mapMutations} from 'vuex'
export default {
  name: "subtraction",
  computed:{
    ...mapState(['count'])
  },
  methods:{
    ...mapMutations(['sub','subN']),
    sub1(){
      this.sub()
    },
    sub2(){
      this.subN(10)
    }
  }
}
</script>
