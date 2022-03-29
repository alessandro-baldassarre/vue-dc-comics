<template>
  <div>
    <div class="footer-menu">
      <div class="my-container">
        <div class="footer-menu-links">
          <div>
            <h5>dc comics</h5>
            <ul>
              <a
                v-for="(link, index) in dcComicsLinks"
                :key="index"
                :href="link.url"
                ><li>{{ link.name }}</li></a
              >
            </ul>
            <h5>shop</h5>
            <ul>
              <a
                v-for="(link, index) in shopLinks"
                :key="index"
                :href="link.url"
                ><li>{{ link.name }}</li></a
              >
            </ul>
          </div>
          <div>
            <h5>dc</h5>
            <ul>
              <a v-for="(link, index) in dcLinks" :key="index" :href="link.url"
                ><li>{{ link.name }}</li></a
              >
            </ul>
          </div>
          <div>
            <h5>sites</h5>
            <ul>
              <a
                v-for="(link, index) in sitesLinks"
                :key="index"
                :href="link.url"
                ><li>{{ link.name }}</li></a
              >
            </ul>
          </div>
        </div>
        <div class="footer-menu-logo">
          <img src="../assets/img/dc-logo-bg.png" alt="dc logo" />
        </div>
      </div>
    </div>
    <div class="footer-bottom">
      <div class="my-container">
        <div class="footer-button">
          <a href="#">sign-up now!</a>
        </div>
        <div class="footer-social">
          <a href="#">follow us</a>
          <a href="#"
            ><img src="../assets/img/footer-facebook.png" alt="facebook logo" />
          </a>
          <a href="#"
            ><img src="../assets/img/footer-twitter.png" alt="twitter logo" />
          </a>
          <a href="#"
            ><img src="../assets/img/footer-youtube.png" alt="yootube logo" />
          </a>
          <a href="#"
            ><img src="../assets/img/footer-pinterest.png" alt="pinterest logo"
          /></a>
          <a href="#"
            ><img src="../assets/img/footer-periscope.png" alt="periscope logo"
          /></a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "IndexFooter",
  data: function () {
    return {
      dcComicsLinks: [
        {
          name: "Characters",
          url: "#",
          active: false,
        },
        {
          name: "Comics",
          url: "#",
          active: false,
        },
        {
          name: "Movies",
          url: "#",
          active: false,
        },
        {
          name: "TV",
          url: "#",
          active: false,
        },
        {
          name: "Games",
          url: "#",
          active: false,
        },
        {
          name: "Videos",
          url: "#",
          active: false,
        },
        {
          name: "News",
          url: "#",
          active: false,
        },
      ],
      dcLinks: [
        {
          name: "Terms Of Use",
          url: "#",
          active: false,
        },
        {
          name: "Privacy policy (New)",
          url: "#",
          active: false,
        },
        {
          name: "Ad Choises",
          url: "#",
          active: false,
        },
        {
          name: "Advertising",
          url: "#",
          active: false,
        },
        {
          name: "Jobs",
          url: "#",
          active: false,
        },
        {
          name: "Subscriptions",
          url: "#",
          active: false,
        },
        {
          name: "Talent Workshops",
          url: "#",
          active: false,
        },
        {
          name: "CPSC Certificates",
          url: "#",
          active: false,
        },
        {
          name: "Ratings",
          url: "#",
          active: false,
        },
        {
          name: "Shop Help",
          url: "#",
          active: false,
        },
        {
          name: "Contact Us",
          url: "#",
          active: false,
        },
      ],
      sitesLinks: [
        {
          name: "DC",
          url: "#",
          active: false,
        },
        {
          name: "MAD Megazine",
          url: "#",
          active: false,
        },
        {
          name: "DC Kids",
          url: "#",
          active: false,
        },
        {
          name: "DC Universe",
          url: "#",
          active: false,
        },
        {
          name: "DC Power Visa",
          url: "#",
          active: false,
        },
      ],
      shopLinks: [
        {
          name: "Shop DC",
          url: "#",
          active: false,
        },
        {
          name: "Shop DC Collectibles",
          url: "#",
          active: false,
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/scss/partials/_variables.scss";

.footer-menu {
  height: 280px;
  background-image: url("../assets/img/footer-bg.jpg");
  overflow: hidden;
  .footer-menu-links {
    display: flex;
    h5 {
      color: white;
      text-transform: uppercase;
      margin-bottom: 0.5rem;
    }
    ul {
      list-style-type: none;
      margin: 0 1.5rem 0.5rem 0;
      padding: 0;
    }
    a {
      font-size: 0.6rem;
      text-decoration: none;
      color: $grayColor;
    }
  }

  .footer-menu-logo {
    img {
      height: 415px;
    }
  }
}

.footer-bottom {
  height: 80px;
  background-color: $lightBlackBgColor;
  .footer-button a {
    color: white;
    text-decoration: none;
    text-transform: uppercase;
    padding: 0.6rem 0.8rem;
    border: 2px solid $primaryColor;
    font-size: 0.7rem;
    font-weight: 600;
  }
  .footer-social {
    a {
      color: $primaryColor;
      text-decoration: none;
      text-transform: uppercase;
      font-size: 0.8rem;
      font-weight: 600;
    }
    img {
      margin: 0 0 0 1rem;
      height: 25px;
      vertical-align: middle;
    }
  }
}
</style>
