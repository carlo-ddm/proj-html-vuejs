<template>
  <header>
    <!-- TOP -->
    <div class="top">
      <div class="cdd_container d-flex justify-content-between align-items-center">

        <div class="tel-contacts">
          <i class="fa-solid fa-phone"></i>
          <span>(001)88451234</span>
          <span>88455438</span>
        </div>

        <!-- social -->
        <div>
          <i class="fa-brands fa-facebook-f"></i>
          <i class="fa-brands fa-twitter"></i>
          <i class="fa-brands fa-pinterest-p"></i>
        </div>

      </div>
    </div>

    <!-- BOTTOM -->
    <div class="bottom">
      <div
        class="cdd_container d-flex justify-content-between align-items-center">
        
        <img src="../assets/images/cropped-Group-39-2x.png" alt="">


        <nav>
          <ul class="m-0 p-0">
            <li v-for="(link, index) in nav" :key="`_link_${index}`">
              <a :href="link.href"> {{ link.pointer }} </a>
            </li>
          </ul>
        </nav>

        <div class="d-flex justify-content-between align-items-center">
          <div class="cd-btn">Purchase</div>
          <i class="fa-solid fa-magnifying-glass"></i>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "HeaderComp",

  data() {
    return {
      // Nav
      nav: [
        {
          pointer: "home",
          href: "#",
        },
        {
          pointer: "about",
          href: "#",
        },
        {
          pointer: "service",
          href: "#",
        },
        {
          pointer: "showcase",
          href: "#",
        },
        {
          pointer: "contact",
          href: "#",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
// Import VARS
@import "../assets/styles/vars";
// Import MIXINES
@import "../assets/styles/mixines";
// Import UTILITIES
@import "../assets/styles/utilities.scss";

header {
  // TOP
  .top {
    height: 35px;
    background-color: #3d3d3d;

    .cdd_container {
      height: 35px;
      background-color: #3d3d3d;
      color: white;

      .tel-contacts {
        i {
          margin-right: 5px;
        }
        span {
          margin-right: 5px;
          font-size: $primary-font;
        }
      }

      div:nth-last-child(1) {
        i {
          font-size: $primary-font;
          margin: 0 5px;
        }
      }
    }
  }

  // BOTTOM
  .bottom {
    height: 80px;
    .cdd_container {
      height: 80px;
      img {
        width: 170px
      }
      ul {
        @include list-style;
        li a {
          @include a-style;
          color: #AAAAAA;
          &:hover {
            color: #555555;
          }
        }
      }
    }

    .cd-btn {
      @include grad;
      margin: 0 20px;
    }

    i {
      color: $primary-color;
    }
  }
}
</style>