<template>
  <main class="container">
    <AppHeader/>
    <AppRestaurantinfo :datasource="fooddata"/>
  </main>
</template>

<script>
import AppHeader from "~/components/AppHeader";
import AppRestaurantinfo from "~/components/AppRestaurantinfo";
import {mapState} from "vuex";

export default {
  components: {
    AppHeader,
    AppRestaurantinfo
  },
  computed: {
    ...mapState(['fooddata'])
  }
};
</script>

<style></style>
