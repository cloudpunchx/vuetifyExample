<template>
    <div>
        <h1>{{name}}</h1>
        <h2>{{address}}</h2>
        <h3>{{phoneNumber}}</h3>
</div>
</template>

<script>
    export default {
        name: "RestaurantCard",
        props: {
            name: String,
            address: String,
            phoneNumber: String
        },
    }
</script>

<style scoped>
div{
    border: 1px solid hotpink;
}
</style>

<!-- data only relevant to 1 component then use in 1 -->
<!-- data in container that needs to share info from other objs -->
<!-- like in restaurant container, its going to delegate all info to each card -->
<!-- so api call must be made in that container, dont duplicate api calls -->
<!-- if every child needs to make api call, then just make api call in parent -->
<!-- the data (no magical rule) if there is something, a collection of info that nobody above in hierarchy uses, then place there -->
<!-- ex home view doesnt care about restaurant list, no other children of home view -->
<!-- will benefit from restaurant list -->
<!-- essentially found apex of hierarchy that needs that info -->
<!-- data can still be passed on to children, but you know it doesnt go "higher than that" -->
<!-- find highest common denominator interested in this data -->

<!-- input ID's - allowed? -->