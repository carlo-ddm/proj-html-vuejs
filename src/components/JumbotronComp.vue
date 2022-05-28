<template>
  <div class="jumbotron">
    <div class="container">
      <div class="row">

        <!-- Colonna 1 -> TESTO -->
        <div class="col-6 cd1">
          <div class="cd_container">
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

            <div class="jumbo-info d-flex">

              <div class="social-nav">
                <ul class="p-0">
                  <li v-for="(social, index) in socialNav" :key="`_social_${index}`"><a :href="social.href">{{social.name}}</a></li>
                </ul>
              </div>

              <div class="cd_container">
                <div class="d-flex cd-btn">

                  <ul>
                    <li
                     v-for="(point, index) in jumboArg" :key="`_index_${index}`"
                     @click="change(index)"
                     class="mx-2">
                     {{point.buttonText}}
                    </li>
                  </ul>

                </div>
              </div>

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
import firstImg from '../assets/images/Group-35-2x.png';
import secondImg from '../assets/images/Group-35-2x.png';
import thirdImg from '../assets/images/Group-35-2x.png';

export default {
  name: 'JumbotronComp',
  data() {
    return {
      selectedIndex: 0,
      
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
      ],

      jumboArg: [
        {
          buttonText: '1',
          src: firstImg,
          jumboText: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Illo sed, molestias corrupti ea debitis nulla consectetur nesciunt accusamus esse consequatur laudantium incidunt accusantium nihil deleniti dicta commodi, cupiditate ratione! Optio ad, cumque delectus iusto fuga dignissimos voluptas inventore nobis velit!'
        },
        {
          buttonText: '2',
          src: secondImg,
          jumboText: 'consequatur laudantium incidunt accusantium nihil deleniti dicta commodi, cupiditate ratione! Optio ad, cumque delectus iusto fuga dignissimos voluptas inventore nobis velit!'
        },
        {
          buttonText: '3',
          src: thirdImg,
          jumboText: 'consequatur laudantium incidunt accusantium nihil deleniti dicta commodi, cupiditate ratione! Optio ad, cumque delectus iusto fuga dignissimos voluptas inventore nobis velit!'
        },
      ],
    }
  },

  methods: {
    change(index){
      this.selectedIndex = index;
      console.log(index);
      console.log(this.selectedIndex);
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

    .cd_container {
      width: 100%;

      .jumbo-focus-on-your-business {
        margin-bottom: 40px;
        h1 {
          font-size: 70px;
        }
      }

      p {
        margin: 40px 0 40px 0px !important;
      }

      button {
        margin: 40px 0 40px 0px;
      }

      .jumbo-info {

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

        .cd_container {
          ul {
            margin: 0;

            @include list-style;
            li {
              text-align: center;
              cursor: pointer;
              border: 1px solid black;
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