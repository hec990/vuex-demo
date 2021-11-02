<template>
  <div>
    <h3>当前最新的count值为：{{count}}</h3>
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
