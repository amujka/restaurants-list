<script lang="ts" setup>
import restaurants from '@/data.json';
import { IRestaurant } from '~~/interface/IRestaurant';

const restaurantsList = ref<IRestaurant[]>(restaurants);
</script>
<template>
  <div class="container">
    <div class="table">
      <div class="column">
        <RestaurantsTableRow :isHeader="true" />
        <template
          v-for="(restaurant, index) in restaurantsList.slice(
            0,
            restaurantsList.length / 2
          )"
          :key="restaurant.id"
        >
          <RestaurantsTableRow
            :name="restaurant.name"
            :rank="restaurant.rank"
            :index="index"
          />
        </template>
      </div>
      <div class="column">
        <RestaurantsTableRow :isHeader="true" />
        <template
          v-for="(restaurant, index) in restaurantsList.slice(
            25,
            restaurantsList.length
          )"
          :key="restaurant.id"
        >
          <RestaurantsTableRow
            :name="restaurant.name"
            :rank="restaurant.rank"
            :index="index"
          />
        </template>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.table {
  display: flex;
  width: 100%;
  max-width: 1024px;
  margin: 0 auto;
  .column {
    flex: 1 0 calc(50% - 20px);
    margin: 0 10px;
  }
}
</style>
