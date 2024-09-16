<script>
export default {
  data() {
    return {

    }
  }
}
</script>

<template>
  <footer>
    <div class="top-footer">
      <div class="container">

        <div class="links">
          LINK DEL FOOTER
        </div>
        <div class="bg-logo">
        </div>

      </div>
    </div>

    <div class="bottom-footer">

    </div>
  </footer>
</template>

<style scoped>
footer {
  color: white;

  .top-footer {
    height: 300px;
    background-image: url("../assets/img/footer-bg.jpg");
    background-size: cover;

    .container {
      height: 100%;
      display: flex;
      justify-content: space-between;
      align-items: stretch;

      .links {
        padding: 2rem;
        flex-basis: 50%;
      }

      .bg-logo {
        flex-basis: 50%;
        background-image: url("../assets/img/dc-logo-bg.png");
        background-position: center;
        background-size: cover;
      }
    }

  }

  .bottom-footer {
    min-height: 80px;
    background-color: black;
  }
}
</style>