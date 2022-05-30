<template>
  <main>
    <!-- SEZIONE 1 -->
    <section id="sect-1" class="d-flex justify-content-center align-items-center">
      <div class="container">
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
      <div class="container">
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
    <div class="bottom container wrapper d-flex flex-wrap justify-content-between">
      <SectionCardsTwo v-for="(item, index) in pics" :key="`_index_${index}`" :item="item" />
    </div>
    <div class="container d-flex justify-content-center">
      <div class="cd-btn">ciao</div>
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
        ]
        
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
    .container {
      height: 200px;
      .col-6.cd2 {
        padding-top: 60px;
      }
    }
  }
  .cd_card {
  flex-basis: 24.5%;
  height: 24.5%;
  margin-bottom: 10px;
  img {
    width: 100%;
  }
}
  .cd-btn {
    display: flex;
    justify-self: center;
    background-color: bisque;
  }
}




</style>