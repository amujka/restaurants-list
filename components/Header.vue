<script lang="ts" setup>

</script>

<template>
<header class="header">
  <h3 class="logo">Restaurantly</h3>
  <ul class="navigation">
    <li>
      <NuxtLink to="/">Home</NuxtLink>
    </li>
  <li>
      <NuxtLink to="/restaurants">Restaurants</NuxtLink>
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
  background-color: rgb(228, 157, 27);
;
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
