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
    <div class="jumbotron">
      <span>CURRENT SERIES</span>
    </div>

    <div class="comics">
      <div class="container">

        <div class="row">
          <Card v-for="(comic, index) in comics" :key="index" :imgUrl="comic.thumb" :comicTitle="comic.series" />
        </div>

        <div class="load-button">
          <a class="load-more" href="#">
            <span>LOAD MORE</span>
          </a>
        </div>

      </div>
    </div>
  </main>
</template>

<style lang="scss" scoped>
main {
  color: white;

  .jumbotron {
    height: 300px;
    background-image: url(../assets/img/jumbotron.jpg);
    background-size: cover;

    span {
      background-color: #0a7cec;
      padding: 1rem;
      font-weight: bold;

      position: relative;
      top: 285px;
      left: 200px;
    }
  }

  .comics {
    background-color: #1c1c1c;
    padding-top: 3rem;
    padding-bottom: 2rem;

    .load-button {
      text-align: center;
      padding-top: 2rem;
    }

    .load-more {
      background-color: #0a7cec;
      padding: 1rem 4rem;
      font-weight: bold;
      color: white;
    }
  }

  .row {
    display: flex;
    flex-wrap: wrap;
    gap: 30px;
  }
}
</style>