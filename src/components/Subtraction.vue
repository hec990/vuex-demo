<template>
  <div>
    <h3>当前最新的count值为：{{count}}</h3>
    <button> -1 </button>
  </div>
</template>

<script lang="js">
import {mapState} from 'vuex'
export default {
  name: "subtraction",
  computed:{
    ...mapState(['count'])
  }
}
</script>
