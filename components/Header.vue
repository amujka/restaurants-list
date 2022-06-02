<script lang="ts" setup>

</script>

<template>
<header class="header">
  <h3 class="logo">Restaurantly</h3>
  <ul class="navigation">
    <li>
      <a href="/">Home</a>
    </li>
  <li>
      <a href="/restaurants">Restaurants</a>
    </li>
  </ul>
</header>

</template>
<style lang="scss" scoped>
.header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 100%;
  margin: 0;
  padding: 10px;
  box-shadow: 0 1px 3px #808080;
  background-color: coral;
  .logo {
    color: #eee;
  }
  .navigation {
    display: flex;
    align-items: center;
    list-style-type: none;
    li {
      padding: 15px;
      a {
        text-decoration: none;
        color: #eee;
      }
    }
  }
}

</style>