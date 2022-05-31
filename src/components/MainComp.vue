<template>
  <main>
    <!-- SEZIONE 1 -->
    <section id="sect-1" class="d-flex justify-content-center align-items-center">
      <div class="cdd_container">
        <div class="row">
  
          <!-- Colonna 1 -> TESTO -->
          <div class="col-6 cd1">
            <div class="cd_container">
              <div class="we-are-here">
                <h1 class="m-0">We are here to
                  <br>
                   make your website
                   <br>
                   look more elegant
                   <br>
                   and stylish
                </h1>
              </div>
              <button class="cd-btn">view all</button>
            </div>
          </div>
  
          <!-- Colonna 2 -> IMMAGINE -->
          <div class="col-6 cd2">
            <!-- CARDS -->
            <div class="wrapper d-flex flex-wrap justify-content-between">
              <SectionCard v-for="(card, index) in cards" :key="`_index_${index}`" :cardItem="card" />
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- SEZIONE 2 -->
    <section id="sect-2" class="d-flex justify-content-center align-items-center">
      <div class="row">
        <div class="col-6 cd1">
          <img class="architect" src="../assets/images/busy-architect-PYVKWM4-1024x872.jpg" alt="">
          <img class="woman" src="../assets/images/businesswoman-analysing-document-P8WSNMC-1024x820.jpg" alt="">
        </div>
        <div class="col-6 cd2">
          <div class="cd_container">
            <div class="learn-more">
               <h1 class="m-0">learn more
                  <br>
                   about our
                   <br>
                   mission
                </h1>
                <div>
                  <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Illo sed, molestias corrupti ea debitis nulla consectetur nesciunt accusamus esse consequatur laudantium incidunt accusantium nihil deleniti dicta commodi, cupiditate ratione! Optio ad, cumque delectus iusto fuga dignissimos voluptas inventore nobis velit!
                  </p>
                </div>
                <button class="cd-btn">readmore</button>
            </div>
          </div>
        </div>
      </div>
  </section>

  <!-- Sezione 3 -->
    <section id="sect-3">
    <div class="top d-flex align-items-end">
      <div class="cdd_container">
        <div class="row">
          <div class="col-6 cd1">
            <h1>our recente web design -----&---- some examples of past projects</h1>
          </div>
          <div class="col-6 cd2 d-flex align-items-center">
            <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Aliquam adipisci ducimus animi pariatur ab, accusantium error commodi hic ut laboriosam facere dicta, assumenda quis rem ea dolores accusamus esse! Laudantium.</p>
          </div>
        </div>
      </div>
    </div>
    <div class="bottom cdd_container wrapper d-flex flex-wrap justify-content-between">
      <SectionCardsTwo v-for="(item, index) in pics" :key="`_index_${index}`" :item="item" />
    </div>
    <div class="container d-flex justify-content-center">
      <div class="cd-btn">ciao</div>
    </div>
  </section>

  <!-- SEZIONE 4 -->
  <!-- TOP -->
  <section id="sect-4">
    <div class="cdd_container top">
      <div>
        <img src="../assets/images/person-with-long-curly-hair-PZ99QM2-2x.jpg" alt="">
        <div>
          ****
        </div>
      </div>

    </div>

    <!-- BOTTOM -->
    <div class="bottom">
      <div class="cdd_container d-flex justify-content-between">
        <div class="cdd-card d-flex flex-column justify-content-center">
          <h1>
            ciao ciao ciao ciao
          </h1>
          <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Eum quasi vero totam, velit ullam hic eveniet est. Cum nobis aut quos in fugit nulla accusantium, unde neque harum impedit quia?</p>
        </div>
        <div class="cdd-card offers">
          <div class="cdd-box">
            <h4>designin</h4>
            <span>all designs</span>
            <div class="price d-flex justify-content-center align-items-center">price</div>
            <ul class="p-0">
              <li>bisosos</li>
              <li>bisosos</li>
              <li>bisosos</li>
              <li>bisosos</li>
              <li>bisosos</li>
          </ul>
          </div>
        </div>
        <div class="cdd-card offers">
          <div class="cdd-box">
            <h4>designin</h4>
            <span>WordPress Projects</span>
            <div class="price d-flex justify-content-center align-items-center">price</div>
            <ul class="p-0">
              <li>bisosos</li>
              <li>bisosos</li>
              <li>bisosos</li>
              <li>bisosos</li>
              <li>bisosos</li>
          </ul>
          </div>
        </div>
        <div class="cdd-card offers">
          <div class="cdd-box">
            <h4>designin</h4>
            <span>Web Products</span>
            <div class="price d-flex justify-content-center align-items-center">
              <span>price</span>
            </div>
            <ul class="p-0">
              <li>bisosos</li>
              <li>bisosos</li>
              <li>bisosos</li>
              <li>bisosos</li>
              <li>bisosos</li>
          </ul>
          </div>
        </div>
      </div>
    </div>
    <!-- lisa -->
    <div class="lisa">
      <div class="overlay">
        <div class="d-flex justify-content-center align-items-center">
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Hic possimus veritatis, maxime unde velit consequuntur accusamus adipisci quia vitae recusandae fugit sint est quod facere doloribus, cumque voluptatem ullam facilis!
          </p>
        </div>

      </div>
    </div>
    <!-- Latest news or our... -->
    <div class="latest">
        <div class="cdd_container d-flex flex-column align-items-center">
          <h1>latest news</h1>
          <div class="cdd_cards d-flex justify-content-between">
            <div class="cdd_card">
              <img src="../assets/images/serious-businesswoman-with-documents-talking-on-P9Q6LX6-1024.jpg" alt="">
              <div class="presentation">
                ciao
              </div>
            </div>
            <div class="cdd_card">
              <img src="../assets/images/Businessman-at-the-desk-in-his-office-resting--1024x768.jpg" alt="">
              <div class="presentation">
                ciao
              </div>
            </div>
            <div class="cdd_card">
              <img src="../assets/images/simple-home-office-with-tree-PBXRXYB-large-1024x768.jpg" alt="">
              <div class="presentation">
                ciao
              </div>
            </div>
          </div>
          <div class="cd-btn">ciaooo</div>
        </div>
      </div>

      <!-- Clients -->
      <div class="clients">
        <div class="cdd_container d-flex justify-content-between">
          <div class="cd-card">
            <div>

            </div>
          </div>
          <div class="cd-card">
            <div>

            </div>
          </div>
        </div>
        <div class="cdd_container">
          <ul class="p-0 d-flex justify-content-between">
            <li>123</li>
            <li>123</li>
            <li>123</li>
            <li>123</li>
            <li>123</li>
          </ul>
        </div>
      </div>
  </section>
  </main>
</template>

<script>
import SectionCard from "../components/section-cards/SectionCard.vue";
import SectionCardsTwo from '../components/section-cards/SectionCardsTwo.vue'

import img1 from '../assets/images/ina-soulis-227104-unsplash-1024x1024.jpg';
import img2 from '../assets/images/sunisa-misa-531163-unsplash-1024x1024.jpg';
import img3 from '../assets/images/355H-1024x1024.jpg';
import img4 from '../assets/images/photo-1448932252197-d19750584e56-1024x1024.jpg';
import img5 from '../assets/images/business-competition-PB366D8-1024x1024.jpg';
import img6 from '../assets/images/cozy-sofa-in-living-room-PQR5AB9-1024x1024.jpg';
import img7 from '../assets/images/aa9a4539-PQGJ7HU-1024x1024.jpg';
import img8 from '../assets/images/cody-davis-253928-unsplash-1024x1024.jpg';


export default {
     data() {
      return {
        cards: [
          {
            icon: 'fa-gauge-simple-high',
            arg: 'speed optimization',
            text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. At earum quam cumque cum quod vero.'
          },
          {
            icon: 'fa-cloud',
            arg: 'cloud solution',
            text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. At earum quam cumque cum quod vero.'
          },
          {
            icon: 'fa-mobile-screen-button',
            arg: 'website design',
            text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. At earum quam cumque cum quod vero.'
          },
          {
            icon: 'fa-clock',
            arg: 'online marketing',
            text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. At earum quam cumque cum quod vero.'
          },
        ],

        pics:[
          {
            pic: img1
          },
          {
            pic: img2
          },
          {
            pic: img3
          },
          {
            pic: img4
          },
          {
            pic: img5
          },
          {
            pic: img6
          },
          {
            pic: img7
          },
          {
            pic: img8
          },
        ],
      }
    },
    components: { SectionCard, SectionCardsTwo }
}
</script>

<style lang="scss" scoped>
// import Vars
@import '../assets/styles/vars';
// import Mixines
@import '../assets/styles/mixines';
// import Utilities
@import '../assets/styles/utilities.scss';


// SEZIONE 1
#sect-1 {
  width: 100%;
  height: 800px;

  .col-6.cd1 {
    padding-top: 130px;

    .cd_container {
      width: 100%;
      .we-are-here {
        margin-bottom: 40px;
      }
    }
  }
}

// SEZIONE 2
#sect-2 {
  width: 100%;
  height: 800px;
  background-color: #F9F9F9;

  .col-6.cd1 {
    position: relative;
    display: flex;
    align-items: center;
    img.architect {
      width: 600px;
      border-radius: 20px;
    }
    img.woman {
      position: absolute;
      left: 180px;
      top: 150px;
      width: 600px;
      border-radius: 20px;
    }
  }

  .col-6.cd2 {
    padding-top: 130px;
    padding-left: 70px;
    .cd_container {

      .learn-more {
        margin-bottom: 40px;
      }

      p {
        margin: 40px 0 40px 0px !important;
      }

       button {
        margin: 40px 0 40px 0px;
      }
    }
  }
}

// SEZIONE 3
#sect-3 {
  width: 100%;
  height: 1500px;
  .top {
    height: calc(20%);
    .cdd_container {
      height: 200px;
      .col-6.cd2 {
        padding-top: 60px;
      }
    }
  }
  .cd-btn {
    display: flex;
    justify-self: center;
    background-color: bisque;
  }
}

#sect-4 {
  width: 100%;
  background-color: #F9F9F9;
  .top {
    padding: 200px 0;
    div {
      position: relative;
      opacity: 0.8;
      background-color: green;
      width: 735px;
      height: 595px;
      border-radius: 20px;
      img {
        opacity: 0.5;
        width: 100%;
        height: 100%;
        border-radius: 20px;
      }
      div {
        position: absolute;
        top: 70px;
        left: 610px;
        border: 1px solid black;
        border-radius: 20px;
        width: 735px;
        height: 595px;
        background-color: white;
        opacity: 1;
      }
    }
  }

  .bottom {
    padding: 150px 0;
    .cdd_container {
      height: 400px;

      .cdd-card {
        flex-basis: calc(100% / 4);
      }

      .offers {
        padding: 0 40px;

        .cdd-box {
          text-align: center;
          border: 1px solid black;
          height: 100%;
          border-radius: 10px;

          .price {
            height: 60px;
            border: 1px solid black;
            background-color: gold;
          }

          ul {
            margin-top: 40px;
            li {
              @include list-style;
              justify-content: center;
              margin: 20px 0px;
              &::before {
                content: '/2713';
                display: inline-block;
                width: 12px;
                height: 12px;
                // background-image: url(img/chevron-down-solid.svg);
                background-position: center;
                line-height: 1px;
                margin-left: 4px;
              }
            }
          } 
        }
      }
    }
  }

  .lisa {
    position: relative;
    width: 100%;
    height: 600px;
    background-image: url(../assets/images/four-businesspeople-in-a-boardroom-with-paperwork-PC4V8H4.jpg);
    background-size: cover;
    background-position: center;
    .overlay {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background-color: rgb(34, 34, 34);
      opacity: 0.8;
      div {
        align-items: center;
        width: 50%;
        height: 100%;
        margin: auto;
        p {
          text-align: center;
          color: white;
        }
      }
    }
  }

  .latest {
    padding: 150px 0;
    border: 1px solid black;

    .cdd_container {
  
      .cdd_cards {
        width: 100%;
      }
      .cdd_card {
        position: relative;
        padding: 20px;
        flex-basis: calc(100% / 3);
       
        img {
          width: 100%;
          border-radius: 5px;
        }
        .presentation {
          position: absolute;
          left: 45px;
          bottom: -25px;
          width: 80%;
          border: 1px solid black;
          border-radius: 5px;
          height: 100px;
          background-color: white;
        }
      }
    }

    .cd-btn {
      margin-top: 70px;
      background-color: rgb(150, 150, 43);
    }
  }

  .clients {
    padding: 150px 0;
    width: 100%;
    .cdd_container {
      .cd-card {
        padding: 10px;
        flex-basis: calc(100% / 2);
        height: 300px;

        div {
          width: 100%;
          height: 100%;
          border: 1px solid black;
          border-radius: 10px;
        }
      
      }
    }

    li {
      @include list-style;
    }
  }


}
</style>