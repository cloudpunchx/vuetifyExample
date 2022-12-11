<template>
<div>
  <!-- you can do cool buttons with icons -->
  <!-- v-icon, instead of putting Click Me, you nest the icon -->
  <!-- always MDI-icon name you take from site -->
  <!-- <v-btn 
  small
  class="deep-purple darken-1"
  elevation="5"><v-icon>mdi-cloud-download</v-icon></v-btn> -->
  <RestaurantContainer/>
</div>
</template>

<script>
import RestaurantContainer from '@/components/RestaurantContainer.vue';

  export default {
    name: 'HomeView',

    components: {
      RestaurantContainer
    },
  }
</script>

<style scoped>
/* PIECE OF ADVICE - BECAUSE BUTTON ISN'T A REAL HTML ELEMENT*/
/* inspect V-BTN in browser, you can see it's actually a class called .v-btn */
.v-btn{
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
  top: 25vh;
}
</style>