<template>
  <div>
    <h3>{{showNum}}</h3>
    <button @click="sub"> -1 </button>
    <button @click="subN(10)"> -N </button>
    <button @click="subAsync">1s后-1</button>
    <button @click="subNAsync(100)">1s后-N</button>
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
  }
}
</script>
