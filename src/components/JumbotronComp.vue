<template>
  <div class="jumbotron">
    <div class="container">
      <div class="row">

        <!-- Colonna 1 -> TESTO -->
        <div class="col-6 cd1">
          <div class="cd-container">
            <div class="jumbo-focus-on-your-business">
              <span>17 years of experience</span>
              <h1 class="m-0">Focus on your
                <br>
                 business
              </h1>
            </div>
            <p class="m-0">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Illo sed, molestias corrupti ea debitis nulla consectetur nesciunt accusamus esse consequatur laudantium incidunt accusantium nihil deleniti dicta commodi, cupiditate ratione! Optio ad, cumque delectus iusto fuga dignissimos voluptas inventore nobis velit!
            </p>

            <button class="cd-btn">readmore</button>

            <div class="social-nav">
              <ul class="p-0">
                <li v-for="(social, index) in socialNav" :key="`_social_${index}`"><a :href="social.href">{{social.name}}</a></li>
              </ul>
            </div>
          </div>
        </div>

        <!-- Colonna 2 -> IMMAGINE -->
        <div class="col-6 cd2">
          <img src="../assets/images/Group-35-2x.png" alt="jumbotron-pic-1">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'JumbotronComp',
  data() {
    return {
      socialNav: [
        {
          name: 'facebook',
          href: '#'
        },
        {
          name: 'instagram',
          href: '#'
        },
        {
          name: 'youtube',
          href: '#'
        },
        {
          name: 'twitter',
          href: '#'
        },
      ]
    }
  },
}
</script>

<style lang="scss" scoped>
//i import Vars
@import '../assets/styles/vars';
// import Mixines
@import '../assets/styles/mixines';
// import Utilities
@import '../assets/styles/utilities.scss';


.jumbotron {
  overflow: hidden;
  height: 800px;
  background-color: #F9F9F9;

  .col-6.cd1{
    padding-top: 130px;

    .cd-container {
      width: 100%;

      .jumbo-focus-on-your-business {
        margin-bottom: 40px;
      }

      p {
        margin: 40px 0 40px 0px !important;
      }

      button {
        margin: 40px 0 40px 0px;
      }

      .social-nav {
        margin: 40px 0 40px 0px;
        ul {
          @include list-style;
          li {
            a {
              @include a-style
            }
          }
        }
      }
    }
  }


  .col-6.cd2 {
    img {
      position: relative;
      top: -170px;
      right: 150px;
      width: 210%;
    }
    }
}


</style>