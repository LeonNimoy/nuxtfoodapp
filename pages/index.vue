<template>
  <main class="container">
    <AppHeader/>
    <AppRestaurantinfo/>
  </main>
</template>

<script>
import AppHeader from "~/components/AppHeader";
import AppRestaurantinfo from "~/components/AppRestaurantinfo";

export default {
  components: {
    AppHeader,
    AppRestaurantinfo
  }
};
</script>

<style></style>
