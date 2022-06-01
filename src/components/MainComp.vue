<template>
  <main>
    <!-- SEZIONE 1 -->
    <section id="sect-1" class="d-flex justify-content-center align-items-center">
      <div class="cdd_container">
        <div class="row">
  
          <!-- Colonna 1 -> TESTO -->
          <div class="col-5 colonna-sinistra d-flex align-items-center">
            <div class="custom_container">
              <div class="we-are-here">
                <h1>we are here to 
                  <br>
                   make your <span>website</span>
                   <br>
                   look more <span>elegant</span>
                   <br>
                   and stylish
                </h1>
              </div>
              <button @click="isActive = !isActive"
              :class="{'active' : isActive}"
              class="cd-btn">view all</button>
            </div>
          </div>
  
          <!-- Colonna 2 -> IMMAGINE -->
          <div class="col-7 colonna-destra">
            <!-- CARDS -->
            <div class="wrapper d-flex flex-wrap justify-content-start">
              <SectionCard v-for="(card, index) in cards" :key="`_index_${index}`" :cardItem="card" />
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- SEZIONE 2 -->
    <section id="sect-2" class="d-flex justify-content-center align-items-center">
      <div class="row">
        <div class="col-6 colonna-sinistra">
          <div class="green-overlay" >
            <img class="architect" src="../assets/images/busy-architect-PYVKWM4-1024x872.jpg" alt="">
          </div>
          <img class="woman" src="../assets/images/businesswoman-analysing-document-P8WSNMC-1024x820.jpg" alt="">
        </div>
        <div class="col-6 colonna-destra d-flex justify-content-center align-items-center">
          <div class="custom_container">
            <div class="learn-more">
               <h1 class="m-0">learn more
                  <br>
                   about our
                   <br>
                   <span>mission</span>
                </h1>
                <div>
                  <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Illo sed, molestias corrupti ea debitis nulla consectetur nesciunt accusamus esse consequatur laudantium incidunt accusantium nihil deleniti dicta commodi, cupiditate ratione! Optio ad, cumque delectus iusto fuga dignissimos voluptas inventore nobis velit!
                  </p>
                </div>
                <button
                @click="isActive2 = !isActive2"
                :class="{'active' : isActive2}"
                class="cd-btn">readmore</button>
            </div>
          </div>
        </div>
      </div>
  </section>

  <!-- Sezione 3 -->
    <section id="sect-3">
      <div class="cdd_container">
        <div class="top d-flex align-items-end">
            <div class="row">
              <div class="col-6 colonna-sinistra">
                <h1>Our recent <span>web design</span> & some examples of past <span>projects</span></h1>
              </div>
              <div class="col-6 colonna-destra d-flex align-items-end">
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Aliquam adipisci ducimus animi pariatur ab, accusantium error commodi hic ut laboriosam facere dicta, assumenda quis rem ea dolores accusamus esse! Laudantium.</p>
              </div>
            </div>
        </div>
        <!-- BOTTOM -> SERIE di IMMAGINI -->
        <div class="bottom wrapper d-flex flex-wrap justify-content-between">
          <SectionCardsTwo v-for="(item, index) in pics" :key="`_index_${index}`" :item="item" />
          <div class="custom_container w-100 d-flex justify-content-center">
            <div
            @click="isActive3 = !isActive3"
            :class="{'active' : isActive3}"
             class="cd-btn">read more</div>
          </div>
        </div>
      </div>
    
  </section>

  <!-- SEZIONE 4 -->
  <!-- TOP -->
  <section id="sect-4">
    <div class="cdd_container top">
      <div class="custom_container w-100">
        <div class="green">
          <div class="long-hair">
            
          </div>
        </div>
      </div>
      <div class="custom_container over w-100">
        <div>
          <h1>we <span>love</span> what <br> we do </h1>
          <p>
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Totam architecto itaque cumque dolore deleniti cupiditate laborum, consequuntur commodi dolores ea laudantium, eaque laboriosam debitis maxime doloribus sint officia dolorem quisquam. Dolore illo quibusdam repudiandae corporis temporibus suscipit natus enim eveniet, exercitationem veritatis aut quasi asperiores magni, dignissimos ducimus quaerat, vel necessitatibus! Deserunt ab illum distinctio, nemo ipsa sunt quasi numquam.
          </p>
          <ul class="p-0">
            <li>Lorem ipsum dolor sit amet consectetur adipisicing elit. Iurer?</li>
            <li>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatum, odit.</li>
            <li>Lorem ipsum dolor sit amet consectetur </li>
          </ul>
        </div>
      </div>
    </div>

    <!-- BOTTOM -->
    <div class="bottom">
      <div class="cdd_container d-flex justify-content-between">
        <div class="cdd-card d-flex flex-column justify-content-center">
          <h1>
            with <span>live chat <br> 24/7 </span> support
          </h1>
          <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Eum quasi vero totam, velit ullam hic eveniet est. Cum nobis aut quos in fugit nulla accusantium, unde neque harum impedit quia?</p>
        </div>
        <div class="cdd-card offers">
          <div class="cdd-box">
            <h4>designin</h4>
            <span>all designs</span>
            <div class="price-black d-flex justify-content-center align-items-center">price</div>
            <ul class="p-0">
              <li><p>Lorem ipsum dolor sit amet.</p></li>
              <li><p>Lorem ipsum dolor sit amet.</p></li>
              <li><p>Lorem ipsum dolor sit amet.</p></li>
              <li><p>Lorem ipsum dolor sit amet.</p></li>
              <li><p>Lorem ipsum dolor sit amet.</p></li>
          </ul>
          </div>
        </div>
        <div class="cdd-card offers">
          <div class="cdd-box">
            <h4>designin</h4>
            <span>WordPress Projects</span>
            <div class="price-green d-flex justify-content-center align-items-center">price</div>
            <ul class="p-0">
              <li><p>Lorem ipsum dolor sit amet.</p></li>
              <li><p>Lorem ipsum dolor sit amet.</p></li>
              <li><p>Lorem ipsum dolor sit amet.</p></li>
              <li><p>Lorem ipsum dolor sit amet.</p></li>
              <li><p>Lorem ipsum dolor sit amet.</p></li>
          </ul>
          </div>
        </div>
        <div class="cdd-card offers">
          <div class="cdd-box">
            <h4>designin</h4>
            <span>Web Products</span>
            <div class="price-black d-flex justify-content-center align-items-center">
              <span>price</span>
            </div>
            <ul class="p-0">
              <li><p>Lorem ipsum dolor sit amet.</p></li>
              <li><p>Lorem ipsum dolor sit amet.</p></li>
              <li><p>Lorem ipsum dolor sit amet.</p></li>
              <li><p>Lorem ipsum dolor sit amet.</p></li>
              <li><p>Lorem ipsum dolor sit amet.</p></li>
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
        active: 'active',
        isActive: false,
        isActive2: false,
        isActive3: false,

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

        boxs: [
          {
            title: 'dev',
            subtitle: 'defr',
            list: [
              {
                item1: 'dfsdfsf',
                item2: 'dfsdfsf',
                item3: 'dfsdfsf',
                item4: 'dfsdfsf',
                item5: 'dfsdfsf',
              }
            ]
          }
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

// CLASSI DINAMICHE
.active {
  box-shadow: 0 0 15px #dedede;
}


// SEZIONE 1
#sect-1 {
  width: 100%;
  height: 800px;

  .col-5.colonna-sinistra {
    .custom_container {
      width: 100%;
      .we-are-here {
        margin-bottom: 40px;
        h1 {
          font-size: 45px;
          font-weight: 300;
          text-transform: capitalize;
          span {
            color: $primary-color;
          }
        }
      }
      .cd-btn {
        @include grad;
      }
    }
  }
}

// SEZIONE 2
#sect-2 {
  width: 100%;
  height: 800px;
  background-color: #F9F9F9;

  .col-6.colonna-sinistra {
    position: relative;
    display: flex;
    align-items: center;
    .green-overlay {
      @include grad;
      border-radius: 20px;
      img.architect {
        width: 600px;
        border-radius: 20px;
        opacity: 0.2;
      }
    }
    img.woman {
      position: absolute;
      left: 210px;
      top: 70px;
      width: 600px;
      border-radius: 20px;
    }
  }

  .col-6.colonna-destra {
    .custom_container {
      width: 60%;
      .learn-more {
        margin-bottom: 40px;
        h1 {
          font-size: 45px;
          font-weight: 300;
          span {
            color: $primary-color
          }
        }
      }

      p {
        margin: 40px 0 40px 0px !important;
        @include paragr
      }

       button {
        margin: 40px 0 40px 0px;
        @include grad
      }
    }
  }
}

// SEZIONE 3
#sect-3 {
  padding: 100px 0 180px;
  width: 100%;
  .cdd_container {
    .top {
      padding-bottom: 50px;
      .colonna-sinistra {
        
        h1 {
          font-size: 45px;
          font-weight: 300;
          span {
            color: $primary-color;
          }
        }
      }

      .colonna-destra {
        p {
          @include paragr
        }
      }
    }
  }

  .custom_container {
    margin: 100px 0 0px;
    .cd-btn {
      @include grad
    }
  }
}

#sect-4 {
  width: 100%;
  background-color: #F9F9F9;
  .top {
    padding: 200px 0 0;
    .custom_container {
      .green {
        @include grad;
        width: 52%;
        border-radius: 10px;
        div.long-hair {
          width: 100%;
          height: 600px;
          border: 1px solid #FFFFFF;
          border-radius: 10px;
          background-image: url(../assets/images/person-with-long-curly-hair-PZ99QM2-2x.jpg);
          background-position: center;
          background-size: cover;
          opacity: 0.2;
        }
      }
    }

    .custom_container.over {
      display: flex;
      justify-content: end;
      position: relative;
      bottom: 550px;
      div {
        width: 53%;
        height: 600px;
        padding: 100px 50px;
        border: 1px solid #FFFFFF;
        border-radius: 10px;
        background-color: white;
        box-shadow: 0 0 15px #dedede;
        h1 {
          font-size: 45px;
          font-weight: 300;
          text-transform: capitalize;
          span {
            color: $primary-color;
          }
        }
        p, ul {
          @include paragr
        }
        ul {
          list-style: none;
          li {
            margin: 10px 0;
            &::before {
              content:'\2713';
              color: $primary-color;
              font-weight: bold;
              position: relative;
              top: 5px;
              right: 6px;
            }
          }
        }
      }
    }
  }

  .bottom {
    .cdd_container {
      padding: 0 0 180px;

      h1 {
        font-size: 45px;
        font-weight: 300;
        
        span {
          color: $primary-color;
        }
      }

      p {
        @include paragr
      }



      .cdd-card {
        flex-basis: calc(100% / 4);
      }

      .offers {
        padding: 0 30px;

        .cdd-box {
          text-align: center;
          border: 1px solid #FFFFFF;
          border-radius: 10px;
          background-color: white;
          box-shadow: 0 0 15px #dedede;
          height: 500px;
          border-radius: 10px;
          .price-black {
            width: 100%;
            height: 80px;
            @include black-grad
          }
          .price-green {
            width: 100%;
            height: 80px;
            @include grad
          }

          ul {
            margin-top: 40px;
            li {
              display: flex;
              list-style: none;
              justify-content: center;
              margin: 10px 0px;
              p {
                @include paragr;
                &::before {
                  content: '\2713';
                  position: relative;
                  right: 5px;
                  background-position: center;
                  color: black;
                  font-size: 14px;
                  font-weight: bold;
                }
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