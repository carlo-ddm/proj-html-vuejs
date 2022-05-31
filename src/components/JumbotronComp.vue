<template>
  <div class="jumbotron">
    <div class="cdd_container">
      <div class="row">

        <!-- Colonna 1 -> TESTO -->
        <div class="col-6 colonna-sinistra">
          <div class="custom-container">
            <div class="jumbo-focus-on-your-business">
              <div>17 years of experience</div>
              <h1 class="m-0">Focus on Your
                <br>
                 <span class="business">Business</span>
              </h1>
            </div>

            <div>
              <div :class="selectedIndex === index ? 'd-block' : 'd-none' " class="custom-container" v-for="(point, index) in jumboArg" :key="`_index1_${index}`">
                <p class="paragr-jumbo" v-if="selectedIndex === index">
                  {{jumboArg[selectedIndex].jumboText}}
                </p>
              </div>
            </div>


            <button class="cd-btn">readmore</button>

            <div class="jumbo-info d-flex align-items-center">

              <div class="social-nav">
                <ul class="p-0">
                  <li v-for="(social, index) in socialNav" :key="`_social_${index}`"><a :href="social.href">{{social.name}}</a></li>
                </ul>
              </div>

              <div class="button-container d-flex justify-content-center align-items-center">
                  <div
                   v-for="(point, index) in jumboArg" :key="`_index2_${index}`"
                   @click="change(index)"
                   class=" d-flex justify-content-center align-items-center mx-2">
                   {{point.buttonText}}
                  </div>
              </div>

        

            </div>

          </div>
        </div>

        <!-- Colonna 2 -> IMMAGINE -->
        <div class="col-6 cd2">
          <div class="cd_container"
          v-for="(point, index) in jumboArg" :key="`_index3_${index}`" >
            <img
            v-if="selectedIndex === index"
            :src="`${jumboArg[selectedIndex].src}`" alt="">
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import firstImg from '../assets/images/Group-35-2x.png';
import secondImg from '../assets/images/Group-36-2x.png';
import thirdImg from '../assets/images/Group-40-2x.png';

export default {
  name: 'JumbotronComp',
  data() {
    return {
      selectedIndex: 0,
      dNone: 'd-none',
      dBlock: 'd-block',

      
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
          buttonText: '01',
          src: firstImg,
          jumboText: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Illo sed, molestias corrupti ea debitis nulla consectetur nesciunt accusamus esse consequatur laudantium incidunt accusantium nihil deleniti dicta commodi, cupiditate ratione! Optio ad, cumque delectus iusto fuga dignissimos voluptas inventore nobis velit!'
        },
        {
          buttonText: '02',
          src: secondImg,
          jumboText: 'consequatur laudantium incidunt accusantium nihil deleniti dicta commodi, cupiditate ratione! Optio ad, cumque delectus iusto fuga dignissimos voluptas inventore nobis velit!'
        },
        {
          buttonText: '03',
          src: thirdImg,
          jumboText: 'consequatur laudantium'
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

// Classi dinamiche
.d-none {
  display: none;
}

.d-Block {
  display: block;
}

// Classi Statiche
.jumbotron {
  overflow: hidden;
  height: 750px;
  background-color: #F9F9F9;

  .col-6.colonna-sinistra{
    padding-top: 130px;

    .custom-container {
      width: 100%;
      height: 50px;

      .jumbo-focus-on-your-business {
        margin-bottom: 40px;
        
        div {
          font-size: $primary-font;
          font-weight: 300;
          color: #00D9A6;
          text-transform: uppercase;
          letter-spacing: 3px;
        }

        h1 {
          font-size: 70px;
          span.business {
            color: #00D9A6;
          }
        }

      }

      .paragr-jumbo {
        @include paragr
      }

      button {
        margin: 40px 0 40px 0px;
        @include black-grad
      }

      .jumbo-info {
        .social-nav {
          margin: 40px 50px 40px 0px;
          ul {
            @include list-style;
            li {
              a {
                  font-size: $paragr-font;
                  text-decoration: none;
                  color: #555555;
                &:after {
                  content:' - '
                }
              }
            }
          }
        }

        .button-container {
          position: relative;
          left: 100px;
          bottom: 18px;
          height: 35px;
          border: none;
          border-radius: 30px;
          cursor: pointer;
          font-size: 10px;
          text-transform: uppercase;
          border: 1px solid black;
          div {
            
            padding: 10px;
            width: 30px;
            height: 30px;
            border-radius: 50%;
            border: 1px solid black;
          }
        }
      }

      }
  }



  .col-6.cd2 {
    .cd_container {
      width: 100%;
      img {
        position: relative;
        top: -170px;
        right: 90px;
        width: 1245px;
        height: 100%;
      }
    }
  }
}


</style>