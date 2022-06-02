<script setup lang="ts" >
    interface IRestaurantRow {
        rank: number
        name: string
    }
    const props = defineProps<IRestaurantRow>()
</script>
<template>
<div class="row">
    <nuxt-link to="#">
        <h4>{{rank}}. {{name}}</h4>
    </nuxt-link>
</div>
</template>

<style lang="scss" scoped>
.row {
    flex: 1 0 calc(50% - 20px);
    margin: 0 10px;
    padding: 10px;
    border-bottom: 1px #eee solid;
    &:nth-child(2n) {
        background-color: #eee;
    }

    a {
        color: coral;
    }
}
</style>