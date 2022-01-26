<template>
  <main class="container">
    <AppHeader/>
    <AppRestaurantInfo :datasource="fooddata"/>
  </main>
</template>

<script>
import AppHeader from "~/components/AppHeader.vue";

export default {
  components: {
    AppHeader,
    AppRestaurantInfo: () =>
      import(/* webpackPrefetch: true */ "~/components/AppRestaurantinfo.vue"),
  },
  computed: {
    fooddata() {
      return this.$store.state.fooddata;
    },
  },
};
</script>

<style></style>
