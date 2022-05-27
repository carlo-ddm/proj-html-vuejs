<template>
  <header>
<!-- TOP -->
    <div class="cd-container-top">
      <div class="container d-flex justify-content-between">
        <span>1</span>
        <!-- social in HTML? -->
        <span>
          <i class="fa-brands fa-facebook-f"></i>
          <i class="fa-brands fa-twitter"></i>
          <i class="fa-brands fa-pinterest-p"></i>
        </span>
      </div>
    </div>

<!-- BOTTOM -->
    <div class="cd-container-bottom d-flex align-items-center">
      <div class="container d-flex justify-content-between align-items-center">

        <span>1</span>

        <nav>
          <ul class="m-0 p-0">
            <li v-for="(link, index) in nav" :key="`_link_${index}`">
              <a :href="link.href"> {{link.pointer}} </a>
            </li>
          </ul>
        </nav>

        <span>3</span>

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

header {
  // TOP
  .cd-container-top {
    width: 100%;
    border-bottom: 1px solid black;
  }
  
  // BOTTOM
  .cd-container-bottom {
    width: 100%;
    height: 80px;
    border-bottom: 1px solid black;

    .container {
      ul {
        @include list-style;
        li a {
          @include a-style
        }
      }
    }
  }
}

</style>