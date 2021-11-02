<template>
  <div>
    <h3>当前最新的count值为：{{this.$store.state.count}}</h3>
    <button> +1 </button>
  </div>
</template>

<script lang="js">
export default {
  name: "addition"
}
</script>
