<script>
export default {
  data() {
    return {
      linkLists: [
        {
          title: 'DC COMICS',
          links: [
            {
              text: 'Characters',
              href: '#',
            },
            {
              text: 'Movies',
              href: '#',
            },
            {
              text: 'TV',
              href: '#',
            },
            {
              text: 'Games',
              href: '#',
            },
            {
              text: 'Videos',
              href: '#',
            },
            {
              text: 'News',
              href: '#',
            },
            {
              text: 'Characters',
              href: '#',
            }
          ]
        },
        {
          title: 'SHOP',
          links: [
            {
              text: 'Shop DC',
              href: '#',
            },
            {
              text: 'Shop DC Collectibles',
              href: '#',
            }
          ]
        },
        {
          title: 'DC',
          links: [
            {
              text: 'Terms Of Use',
              href: '#',
            },
            {
              text: 'Privacy policy (New)',
              href: '#',
            },
            {
              text: 'Ad Choices',
              href: '#',
            },
            {
              text: 'Advertising',
              href: '#',
            },
            {
              text: 'Jobs',
              href: '#',
            },
            {
              text: 'Subscriptions',
              href: '#',
            },
            {
              text: 'Talent Workshops',
              href: '#',
            },
            {
              text: 'CPSC Certificates',
              href: '#',
            },
            {
              text: 'Ratings',
              href: '#',
            },
            {
              text: 'Shop Help',
              href: '#',
            },
            {
              text: 'Contact Us',
              href: '#',
            }
          ]
        },
        {
          title: 'SITES',
          links: [
            {
              text: 'DC',
              href: '#',
            },
            {
              text: 'MAD Magazine',
              href: '#',
            },
            {
              text: 'DC Kids',
              href: '#',
            },
            {
              text: 'DC Universe',
              href: '#',
            },
            {
              text: 'DC Power Visa',
              href: '#',
            }
          ]
        },
      ]
    }
  }
}
</script>

<template>
  <footer>
    <div class="top-footer">
      <div class="container">

        <div class="links">
          <div class="list" v-for="list in linkLists">
            <h3>{{ list.title }}</h3>

            <ul>
              <li v-for="link in list.links">
                <a :href="link.href">{{ link.text }}</a>
              </li>
            </ul>

          </div>
        </div>


        <div class="bg-logo"></div>

      </div>
    </div>

    <div class="bottom-footer">

      <div class="container">

        <div class="sign-up-button">
          <a href="#">
            <span>SIGN-UP NOW!</span>
          </a>
        </div>

        <div class="socials">
          <span>FOLLOW US</span>
          <div class="icons">
            <img src="../assets/img/footer-facebook.png" alt="Facebook">
            <img src="../assets/img/footer-twitter.png" alt="Twitter">
            <img src="../assets/img/footer-youtube.png" alt="Youtube">
            <img src="../assets/img/footer-pinterest.png" alt="Pinterest">
            <img src="../assets/img/footer-periscope.png" alt="Periscope">
          </div>
        </div>

      </div>

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
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;
        gap: 0.5rem;

        .list {
          margin-right: 2rem;

          h3 {
            margin-bottom: 0.5rem;
          }
        }

        a {
          color: gray;
          font-size: 0.8rem;
        }
      }

      .bg-logo {
        flex-basis: 40%;
        background-image: url("../assets/img/dc-logo-bg.png");
        background-position: center;
        background-size: cover;
      }
    }

  }

  .bottom-footer {
    height: 80px;
    background-color: black;

    a {
      color: white;
      border: 1px solid #0a7cec;
      padding: 1rem;
    }

    .container {
      height: 100%;
      display: flex;
      justify-content: space-between;
      align-items: center;

      .socials {
        display: flex;
        gap: 1rem;
        align-items: center;

        span {
          color: #0a7cec;
          font-weight: bolder;
        }

        .icons img {
          margin-right: 1rem;
        }
      }

    }
  }
}
</style>