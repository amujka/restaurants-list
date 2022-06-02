<script setup lang="ts">
interface IRestaurantRow {
  rank?: number;
  name?: string;
  index?: number;
  isHeader?: Boolean;
}
const props = defineProps<IRestaurantRow>();
</script>
<template>
  <div class="row" v-if="isHeader">
    <h4 class="header">Rank</h4>
    <h4 class="header">Chain</h4>
  </div>
  <div v-else class="row" :class="index % 2 !== 0 ? 'bgGray' : null">
    <h4 class="header">{{ rank }}.</h4>
    <nuxt-link :to="`/restaurants/${name}`">
      <h4 class="">{{ name }}</h4>
    </nuxt-link>
  </div>
</template>

<style lang="scss" scoped>
.row {
  display: flex;
  align-items: center;
  padding: 10px;
  border-bottom: 1px #eee solid;
  .header {
    flex-basis: 50px;
    margin: 0;
    margin-right: 2rem;
    color: #404040;
  }

  a {
    color: coral;
  }
}
.bgGray {
  background-color: #eee;
}
</style>
