<script>
export default {
  data() {
    return {
      linkList: [
        {
          text: 'CHARACTERS',
          href: '#',
          active: false
        },
        {
          text: 'COMICS',
          href: '#',
          active: false
        },
        {
          text: 'MOVIES',
          href: '#',
          active: false
        },
        {
          text: 'TV',
          href: '#',
          active: false
        },
        {
          text: 'GAMES',
          href: '#',
          active: false
        },
        {
          text: 'COLLECTIBLES',
          href: '#',
          active: false
        },
        {
          text: 'VIDEOS',
          href: '#',
          active: false
        },
        {
          text: 'FANS',
          href: '#',
          active: false
        },
        {
          text: 'NEWS',
          href: '#',
          active: false
        },
        {
          text: 'SHOP',
          href: '#',
          active: false
        },
      ]
    }
  }
}
</script>

<template>
  <header>
    <div class="container">
      <div class="logo">
        <a href="#">
          <img src="../assets/img/dc-logo.png" alt="Header Logo">
        </a>
      </div>

      <div class="links">
        <ul>
          <li v-for="link in linkList">
            <a :href="link.href"> {{ link.text }} </a>
          </li>
        </ul>
      </div>
    </div>
  </header>
</template>

<style scoped>
.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem;

  .logo {

    img {
      height: 80px;
    }
  }

  .links {

    ul {
      display: flex;
      flex-wrap: wrap;

      li {
        margin-right: 1rem;
        font-weight: bold;
      }
    }
  }
}
</style>