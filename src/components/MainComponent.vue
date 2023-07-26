<script>
export default {
  name: "MainComponent",
  data() {
    return {
      currentSlide: 0,
      visibleSlides: 5, // Numero di immagini visualizzate contemporaneamente nel carosello
      slides: [
        {
          image: new URL('../assets/images/spring_printed_dress-200x260.jpg', import.meta.url).href,
        },
        {
          image: new URL('../assets/images/modern_love_tee-200x260.jpg', import.meta.url).href,
        },
        {
          image: new URL('../assets/images/black_leather_jacket-200x260.jpg', import.meta.url).href,
        },
        {
          image: new URL('../assets/images/black_leather_suit-200x260.jpg', import.meta.url).href,
        },
        {
          image: new URL('../assets/images/hipster_black_top-200x260.jpg', import.meta.url).href,
        },
        {
          image: new URL('../assets/images/blue_jacket_and_white_stripe_tee-200x260.jpg', import.meta.url).href,
        },
        {
          image: new URL('../assets/images/black_elegant_leather_jacket-200x260.jpg', import.meta.url).href,
        },
        {
          image: new URL('../assets/images/blue_leather_jacket-200x260.jpg', import.meta.url).href,
        },
      ],
      currentSlideNewArrivals: 0,
      slidesNewArrivals: [
        {
        image: new URL('../assets/images/spring_printed_dress-400x520.jpg', import.meta.url).href,
        },
        {
        image: new URL('../assets/images/modern_love_tee-400x520.jpg', import.meta.url).href,
        },
        {
        image: new URL('../assets/images/black_leather_jacket-400x520.jpg', import.meta.url).href,
        },
        {
        image: new URL('../assets/images/black_leather_suit-400x520.jpg', import.meta.url).href,
        },
        {
        image: new URL('../assets/images/hipster_black_top-400x520.jpg', import.meta.url).href,
        },
        {
        image: new URL('../assets/images/blue_jacket_and_white_stripe_tee-400x520.jpg', import.meta.url).href,
        },
        {
        image: new URL('../assets/images/black_elegant_leather_jacket-400x520.jpg', import.meta.url).href,
        },
        {
        image: new URL('../assets/images/blue_leather_jacket-400x520.jpg', import.meta.url).href,
        },
      ],
    };
  },
  methods: {
    nextSlide() {
      if (this.currentSlide < this.slides.length - this.visibleSlides) {
        this.currentSlide++;
      }
    },
    prevSlide() {
      if (this.currentSlide > 0) {
        this.currentSlide--;
      }
    },

    nextSlideNewArrivals() {
      if (this.currentSlideNewArrivals < this.slidesNewArrivals.length - this.visibleSlides) {
        this.currentSlideNewArrivals++;
      }
    },
    prevSlideNewArrivals() {
      if (this.currentSlideNewArrivals > 0) {
        this.currentSlideNewArrivals--;
      }
    },
  },
};
</script>

<template>
    <main>
        <section class="jumbo d-flex align-items-center justify-content-center">
            <div class="new-product text-center p-3">
            <h1 class="mb-3">Brand New Arrivals</h1>
            <h3 class="mb-3">NEW COLLECTION FROM NEW YORK</h3>
            <a href="#" class="button">
                VIEW ALL
            </a>
            <a href="#" class="button">
                LOOKBOOK
            </a>
        </div>
        </section>
        <section class="featured-products bg-white text-center">
            <h3 class="mb-2 pt-5">Featured Products</h3>
            <p class="mb-5">Must have products from our top sellers</p>
            <a href="#" class="active-tab">
                Men
            </a>
            <a href="#" class="tab">
                Women
            </a>
            <a href="#" class="tab">
                Accessories
            </a>
            <div class="container mt-5">
                <div class="row justify-content-center">
                    <div class="col-auto text-start">
                        <img src="../assets/images/black_elegant_leather_jacket-200x260.jpg" alt="">
                        <h6 class="mb-1 mt-2">Black Leather Jacket</h6>
                        <p class="mb-1">Men. Jackets. Jeans</p>
                        <span class="discount">$235</span>
                        <span>  $200</span>
                    </div>
                    <div class="col-auto text-start">
                        <img src="../assets/images/black_leather_suit-200x260.jpg" alt="">
                        <h6 class="mb-1 mt-2">Black Leather Jacket</h6>
                        <p class="mb-1">Men. Jackets. Jeans</p>
                        <span>$178</span>
                    </div>
                    <div class="col-auto text-start">
                        <img src="../assets/images/blue_leather_jacket-200x260.jpg" alt="">
                        <h6 class="mb-1 mt-2">Black Leather Jacket</h6>
                        <p class="mb-1">Men. Jackets. Jeans</p>
                        <span>$580</span>
                    </div>
                    <div class="col-auto text-start">
                        <img src="../assets/images/modern_black_leather_suit-200x260.jpg" alt="">
                        <h6 class="mb-1 mt-2">Black Leather Jacket</h6>
                        <p class="mb-1">Men. Jackets. Jeans</p>
                        <span>$96</span>
                    </div>
                </div>
            </div>
        </section>
        <section class="collection">
            <div class="row">
                <div class="col-4 winter">
                    <div class="description text-center">
                        <h1 class="mb-3">Winter Collection</h1>
                        <h3 class="mb-3">STYLISH AND WARM</h3>
                        <a href="#" class="button">
                            VIEW MORE
                        </a>
                    </div>
                </div>
                <div class="col-4 spring">
                    <div class="description text-center">
                        <h1 class="mb-3">Spring Collection</h1>
                        <h3 class="mb-3">BRIGHT AND COLORFUL</h3>
                        <a href="#" class="button">
                            VIEW MORE
                        </a>
                    </div>
                    
                </div>
                <div class="col-4 autumn">
                    <div class="description text-center">
                        <h1 class="mb-3">Autumn Collection</h1>
                        <h3 class="mb-3">RICH AND COMFORTABLE</h3>
                        <a href="#" class="button">
                            VIEW MORE
                        </a>
                    </div>
                    
                </div>
            </div>

        </section>
        <section class="best-seller bg-white text-center p-3">
            <div class="container">
                <h3 class="mb-2 pt-5">Best Seller</h3>
                <p class="mb-5">Must have products from our top sellers</p>
                <div class="slider-wrapper d-flex justify-content-center">
                    <button class="prev-btn" @click="prevSlide" v-show="currentSlide > 0">
                        <i class="fa-solid fa-chevron-left" style="color: #ffffff;"></i>
                    </button>
                    <div v-for="(slide, index) in slides.slice(currentSlide, currentSlide + visibleSlides)" :key="index" class="item" :class="{ active: index === currentSlide }">
                        <img :src="slide.image" alt="">
                    </div>
                    <button class="next-btn" @click="nextSlide" v-show="currentSlide < slides.length - visibleSlides">
                        <i class="fa-solid fa-chevron-right fa-sm" style="color: #ffffff;"></i>
                    </button>
                </div>
            </div>
        </section>
        <section class="shipping">
            <div class="container p-5">
                <div class="row justify-content-between">
                    <div class="col-6">
                        <img src="../assets/images/promo_box_1_bg.jpg" alt="">
                        <div class="cta">
                            <h1 class="mb-3">70% Off</h1>
                            <h3 class="mb-3">Lorem ipsum dolor sit.</h3>
                            <a href="#" class="button">
                                VIEW MORE
                            </a>
                        </div>
                    </div>
                    <div class="col-6">
                        <img src="../assets/images/promo_box_2_bg.jpg" alt="">
                        <div class="cta">
                            <h1 class="mb-3">Free Shipping</h1>
                            <h3 class="mb-3">Lorem ipsum dolor sit.</h3>
                            <a href="#" class="button">
                                VIEW MORE
                            </a>
                        </div>
                        
                    </div>
                </div>
            </div> 
        </section>
        <section class="best-seller bg-white text-center p-3">
            <h3 class="mb-2 pt-5">New Arrivals</h3>
            <p class="mb-5">Must have products from our top sellers</p>
            <div class="slider-wrapper d-flex justify-content-center">
                <button class="prev-btn" @click="prevSlideNewArrivals" v-show="currentSlideNewArrivals > 0">
                    <i class="fa-solid fa-chevron-left" style="color: #ffffff;"></i>
                </button>
                <div v-for="(slide, index) in slidesNewArrivals.slice(currentSlideNewArrivals, currentSlideNewArrivals + visibleSlides)" :key="index" class="item" :class="{ active: index === currentSlideNewArrivals }">
                    <img :src="slide.image" alt="">
                </div>
                <button class="next-btn" @click="nextSlideNewArrivals" v-show="currentSlideNewArrivals < slidesNewArrivals.length - visibleSlides">
                    <i class="fa-solid fa-chevron-right fa-sm" style="color: #ffffff;"></i>
                </button>
            </div>
        </section>
        
        
    </main>
</template>

<style lang="scss" scoped>
@use "../assets/scss/partials/variables.scss" as *;
    .button{
        text-decoration: none;
        background-color: transparent;
        border-radius: 30px;
        padding: 10px 20px;
        border: 1px solid white;
        color: white;
        font-size: 0.8rem;
        font-weight: 400;
    }
    .jumbo {
        background-image: url(../assets/images/home1_slide_three_bg_2.jpg);
        background-size: cover;
        height: 500px;
    }
    .new-product {
        a {
            margin-left: 10px;
        }
        h1 {
            font-weight: 800;
            color: white;
        }
        h3 {
            font-weight: 200;
            color: white;
        }
    }
    .featured-products {
        padding-bottom: 150px;
        .active-tab{
            text-decoration: none;
            padding: 15px 30px;
            background-color: white;
            color: black;
            font-weight: 600;
        }
        .tab{
            text-decoration: none;
            padding: 10px 40px;
            background-color: rgb(238, 233, 233);
            color: black;
            font-weight: 600;
        }
        h3 {
            font-weight: bold;
            font-size: 2.3rem;
        }
        a {
            display: inline-block;
            border: 0.5px solid lightgrey;
        }
        .col-auto {
            h6 {
                font-weight: bold;
            }
            p {
                font-weight: 300;
                font-size: 0.8rem;
            }
            span {
                color: #428cdd;
            }
            .discount {
                text-decoration: line-through;
                font-size: 0.8rem;
            }
        }
    }

    .collection {
        .winter {
            background-image: url(../assets/images/winter_collection_bg.jpg);
            background-size: cover;
            background-repeat: no-repeat;
            height: 500px;
            position: relative;
            .description{
                    position: absolute;
                    bottom: 70px;
                    left: 100px;
                    h1 {
                        color: white;
                        font-size: 1.8rem;
                        font-weight: bold;   
                    }
                    h3 {
                        font-size: 1rem;
                        color: white;
                    }
                }
        }
        .spring {
            background-image: url(../assets/images/spring_collection_bg.jpg);
            background-size: cover;
            background-repeat: no-repeat;
            height: 500px;
            position: relative;
            .description{
                    position: absolute;
                    bottom: 70px;
                    left: 100px;
                    h1 {
                        color: white;
                        font-size: 1.8rem;
                        font-weight: bold;   
                    }
                    h3 {
                        font-size: 1rem;
                        color: white;
                    }
                }
        }
        .autumn {
            background-image: url(../assets/images/autumn_collection_bg.jpg);
            background-size: cover;
            background-repeat: no-repeat;
            height: 500px;
            position: relative;
            .description{
                    position: absolute;
                    bottom: 70px;
                    left: 100px;
                    h1 {
                        color: white;
                        font-size: 1.8rem;
                        font-weight: bold;   
                    }
                    h3 {
                        font-size: 1rem;
                        color: white;
                    }
                }
        }
    }

    .best-seller {
        .slider-wrapper {
            position: relative;
        }
        h3 {
            font-weight: bold;
        }
        .prev-btn, .next-btn {
            width: 20px;
            height: 40px;
            margin: 10px 0;
            background: #ccc;
            cursor: pointer;
            color: white;
            border: none;
        }
        .prev-btn {
            position: absolute;
            left: 20px;
            top: 100px;
        }
        .next-btn {
            position: absolute;
            right: 20px;
            top: 100px;
        }
    }

    .shipping {
        background-image: url(../assets/images/bkgd_confetti-compressor.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        background-position-y: center;
        .col-6 {
            height: 400px;
            position: relative;
            img {
                height: 100%;
            }
            .cta {
                color: white;
                position: absolute;
                left: 80px;
                top: 120px;
                h1 {
                    font-weight: bold;
                }
                h3 {
                    font-size: 14px;
                }
            }
        }
    }



</style>