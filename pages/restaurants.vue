<template>
  <main class="container restaurant">
    <div class="restaurantheading">
      <h1>Restaurants</h1>

      <AppSelect @change="selectedRestaurant = $event"/>
      <pre>{{ $data }}</pre>
    </div>
    <AppRestaurantinfo/>
  </main>
</template>

<script>
import AppRestaurantinfo from "~/components/AppRestaurantinfo";
import AppSelect from "@/components/AppSelect";

export default {
  components: {
    AppRestaurantinfo,
    AppSelect
  },
  data() {
    return {
      selectedRestaurant: ''
    }
  }
};
</script>

<style lang="scss" scoped></style>
