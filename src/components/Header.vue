<template>
  <div id="header">
    <div class="my-container">
      <div class="logo">
        <img src="../assets/img/dc-logo.png" alt="dc logo" />
      </div>
      <div class="header-nav">
        <ul>
          <li
            v-for="(link, index) in headerNavLink"
            :key="index"
            :class="{ active: link.active }"
            @click="clickedLink(index)"
          >
            <a :href="link.url"></a>{{ link.name }}
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "IndexHeader",
  data: function () {
    return {
      headerNavLink: [
        {
          name: "characters",
          url: "#",
          active: false,
        },
        {
          name: "comics",
          url: "#",
          active: true,
        },
        {
          name: "movies",
          url: "#",
          active: false,
        },
        {
          name: "tv",
          url: "#",
          active: false,
        },
        {
          name: "games",
          url: "#",
          active: false,
        },
        {
          name: "collectibles",
          url: "#",
          active: false,
        },
        {
          name: "videos",
          url: "#",
          active: false,
        },
        {
          name: "fans",
          url: "#",
          active: false,
        },
        {
          name: "news",
          url: "#",
          active: false,
        },
        {
          name: "shop",
          url: "#",
          active: false,
        },
      ],
    };
  },
  methods: {
    clickedLink: function (indexClicked) {
      this.headerNavLink.forEach((element, index) => {
        if (indexClicked === index) {
          element.active = true;
          console.log("cliccato");
        } else {
          element.active = false;
          console.log("non cliccato");
        }
      });
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/scss/partials/_variables.scss";
div#header {
  height: 85px;
  .logo {
    img {
      height: 60px;
    }
  }

  .header-nav {
    height: 100%;
    ul {
      height: 100%;
      display: flex;
      list-style-type: none;
      margin: 0;
      li {
        margin: 0 0.5rem;
        line-height: 85px;
        text-transform: uppercase;
        font-size: 0.65rem;
        cursor: pointer;

        &:hover {
          color: $primaryColor;
          border-bottom: 5px solid $primaryColor;
        }
      }
      .active {
        color: $primaryColor;
        border-bottom: 5px solid $primaryColor;
      }
    }
  }
}
</style>
