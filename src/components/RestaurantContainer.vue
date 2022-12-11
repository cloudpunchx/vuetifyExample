<template>
    <div>
        <RestaurantCard/>
    </div>
</template>

<script>
import RestaurantCard from '@/components/RestaurantCard.vue';

    export default {
        name: "RestaurantContainer",
        components: {
            RestaurantCard
        },
        data() {
            return {
                name: "RestaurantContainer"
            }
        },
    }
</script>

<style scoped>

</style>