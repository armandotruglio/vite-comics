<script>
import UserData from "../../dc-comics.json";
import Card from "./Card.vue"

export default {
  data() {
    return {
      comics: UserData,
    }
  },
  components: {
    Card,
  }
}
</script>

<template>
  <main>
    <div class="container">
      <Card v-for="(comic, index) in comics" :key="index" :imgUrl="comic.thumb" :comicTitle="comic.series" />
    </div>
  </main>
</template>

<style scoped>
main {
  color: white;
  background-color: black;
  padding: 4rem;

  .container {
    display: flex;
    flex-wrap: wrap;
  }
}
</style>