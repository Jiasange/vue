<template>
  <div id="nav">
    <template v-for="i in 11">
      <div :key="i">
        <router-link :to="`/1.${i}`">part {{ `1.${i}` }}</router-link>
      </div>
    </template>
  </div>
</template>

<script>
export default {
  name: "Home"
};
</script>

<style lang="less">
#nav {
  padding: 30px;
  a {
    font-weight: bold;
    color: #2c3e50;
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
