<script lang="ts" setup>
    import  restaurants from '@/data.json'
    import { IRestaurant } from '~~/interface/IRestaurant';

    const restaurantsList= ref<IRestaurant[]>(restaurants);
</script>
<template>
    <h1>TOP 50: THE RANKING</h1>
    <div class="table">
        <template v-for="restaurant in restaurantsList" :key="restaurant.id">
            <RestaurantsTableRow
                :name="restaurant.name"
                :rank="restaurant.rank"

            />
        </template>
    </div>
</template>

<style lang="scss" scoped>
.table {
    flex-wrap: wrap;
    display: flex;
    max-width: 1024px;
    margin: 0 auto;

}

</style>