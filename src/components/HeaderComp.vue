<template>
  <header>
<!-- TOP -->
    <div class="cd-container-top d-flex align-items-center">
      <div class="cdd_container d-flex justify-content-between">
        <div>
          <i class="fa-solid fa-phone"></i>
          <span>
            (001)88451234 88455438
          </span>
        </div>
        <!-- social in HTML? -->
        <div>
          <i class="fa-brands fa-facebook-f"></i>
          <i class="fa-brands fa-twitter"></i>
          <i class="fa-brands fa-pinterest-p"></i>
        </div>
      </div>
    </div>

<!-- BOTTOM -->
    <div class="cd-container-bottom d-flex align-items-center">
      <div class="cdd_container d-flex justify-content-between align-items-center">

        <div>
          LOGO
          <span>Phlox</span>
          <span>Business</span>
        </div>

        <nav>
          <ul class="m-0 p-0">
            <li v-for="(link, index) in nav" :key="`_link_${index}`">
              <a :href="link.href"> {{link.pointer}} </a>
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
  name: 'HeaderComp',

  data() {
    return {

      // Nav
      nav: [
        {
          pointer: 'home',
          href: '#'
        },
        {
          pointer: 'about',
          href: '#'
        },
        {
          pointer: 'service',
          href: '#'
        },
        {
          pointer: 'showcase',
          href: '#'
        },
        {
          pointer: 'contact',
          href: '#'
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
// Import VARS
@import '../assets/styles/vars';
// Import MIXINES
@import '../assets/styles/mixines';
// Import UTILITIES
@import '../assets/styles/utilities.scss';

header {
  

  // TOP
  .cd-container-top {
    width: 100%;
    height: 35px;
    background-color: #3D3D3D;
    color: white;

    span {
      margin-left: 2px;
      font-size: $primary-font;
    }
    
    div:nth-last-child(1) {
      i {
        margin: 0 5px;
      }
    }
  }
  
  // BOTTOM
  .cd-container-bottom {
    width: 100%;
    height: 80px;

    .cdd_container {
      width: 100%;
      ul {
        @include list-style;
        li a {
          @include a-style
        }
      }
    }

    .cd-btn {
      background-color: bisque;
    }
  }
}

</style>