<template>
  <div>
    <div class="footer-menu">
      <div class="container">
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
    <div class="footer-bottom"></div>
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
.container {
  width: 67%;
  height: 100%;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.footer-menu {
  height: 280px;
  background-image: url("../assets/img/footer-bg.jpg");
  overflow: hidden;
  .footer-menu-links {
    display: flex;
    h5 {
      color: white;
      text-transform: uppercase;
      margin-bottom: .5rem;
    }
    ul {
      list-style-type: none;
      margin: 0 1.5rem 0 0;
      padding: 0;
    }
    a {
      font-size: 0.6rem;
      text-decoration: none;
      color: rgb(121, 121, 121);
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
  background-color: rgb(42, 42, 42);
}
</style>
