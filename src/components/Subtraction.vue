<template>
  <div>
<!--    <h3>当前最新的count值为：{{count}}</h3>-->
<!--    <h3>{{$store.getters.showNum}}</h3>-->
    <h3>{{showNum}}</h3>
    <button @click="sub1"> -1 </button>
    <button @click="sub2"> -N </button>
    <button @click="sub3">1s后-1</button>
    <button @click="sub4">1s后-N</button>
  </div>
</template>

<script lang="js">
import {mapState,mapMutations,mapActions,mapGetters} from 'vuex'
export default {
  name: "subtraction",
  computed:{
    ...mapState(['count']),
    ...mapGetters(['showNum']),
  },
  methods:{
    ...mapMutations(['sub','subN']),
    ...mapActions(['subAsync','subNAsync']),
    sub1(){
      this.sub()
    },
    sub2(){
      this.subN(10)
    },
    sub3(){
      this.subAsync()
    },
    sub4(){
      this.subNAsync(100)
    },
  }
}
</script>
