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

      testimonials: [
        {
          image: new URL('../assets/images/man_testimonial.png', import.meta.url).href,
          text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Rerum necessitatibus nesciunt non nihil veritatis excepturi amet enim, quo repellat dolorem, quisquam sit perferendis deserunt velit quam culpa, cum accusantium blanditiis.',
          name: 'Dario Pineda. Theme Fusion',
        },
        {
          image: new URL('../assets/images/woman_testimonial.png', import.meta.url).href,
          text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Rerum necessitatibus nesciunt non nihil veritatis excepturi amet enim, quo repellat dolorem, quisquam sit perferendis deserunt velit quam culpa, cum accusantium blanditiis.',
          name: 'Marta Pineda. Theme Fusion',
        },
        // Aggiungi altri testimoni se necessario
      ],

        currentTestimonialIndex: 0,
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

    changeTestimonial(index) {
        this.currentTestimonialIndex = index;
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
        <section class="new-arrivals bg-white text-center p-3">
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
        <section class="testimonial d-flex justify-content-center align-items-center">
            <div class="wrapper">
                <img :src="testimonials[currentTestimonialIndex].image" alt="">
                <p>
                {{ testimonials[currentTestimonialIndex].text }}
                </p>
                <h4>{{ testimonials[currentTestimonialIndex].name }}</h4>
                <div class="circle-container">
                    <span
                        v-for="(testimonial, index) in testimonials"
                        :key="index"
                        class="circle"
                        :class="{ active: index === currentTestimonialIndex }"
                        @click="changeTestimonial(index)"
                    ></span>
                </div>
            </div>
        </section>
        <section class="blog bg-white text-center">
            <h3 class="mb-2 pt-5">From Our Blog</h3>
            <p class="mb-5">The latest Classic Shop News</p>
            <div class="container text-start">
                <div class="row">
                    <div class="col-4 text-center">
                        <img src="../assets/images/post_img_12-320x202.jpg" alt="">
                        <h6 class="mt-3">Lorem ipsum dolor sit amet.</h6>
                        <span>
                            September 9Th, 2023 I 0 Comments
                        </span>
                        <p>
                            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Totam, officia?
                        </p>
                    </div>
                    <div class="col-4 text-center">
                        <img src="../assets/images/post_img_11-320x202.jpg" alt="">
                        <h6 class="mt-3">Lorem ipsum dolor sit amet.</h6>
                        <span>
                            September 9Th, 2023 I 0 Comments
                        </span>
                        <p>
                            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Totam, officia?
                        </p>
                    </div>
                    <div class="col-4 text-center">
                        <img src="../assets/images/post_img_10-320x202.jpg" alt="">
                        <h6 class="mt-3">Lorem ipsum dolor sit amet.</h6>
                        <span>
                            September 9Th, 2023 I 0 Comments
                        </span>
                        <p>
                            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Totam, officia?
                        </p>
                    </div>
                </div>
                
            </div>
            <hr>
        </section>
        <section class="suggested-product">
            <div class="container">
                <div class="row">
                    <div class="col-3 text-black">
                        <h5 class="mb-5">FEATURED</h5>
                        <div class="cards d-flex justify-content-between mb-2">
                            <div class="description">
                                <h6>
                                    Black Jacket
                                </h6>
                                <h6>
                                    $125
                                </h6>
                            </div>
                            <div class="poster">
                                <img src="../assets/images/black_leather_jacket-120x156.jpg" alt="">
                            </div>
                        </div>
                        <hr>
                        <div class="cards d-flex justify-content-between mb-2">
                            <div class="description">
                                <h6>
                                    Black Leather Jacket
                                </h6>
                                <div class="stars">
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                </div>
                                <h6>
                                    $200
                                </h6>
                            </div>
                            <div class="poster">
                                <img src="../assets/images/black_elegant_leather_jacket-120x156.jpg" alt="">
                            </div>
                        </div>
                        <hr>
                        <div class="cards d-flex justify-content-between">
                            <div class="description">
                                <h6>
                                    Hipster Black Top
                                </h6>
                                <h6>
                                    $57
                                </h6>
                            </div>
                            <div class="poster">
                                <img src="../assets/images/hipster_black_top-120x156.jpg" alt="">
                            </div>
                        </div>
                        <hr>
                    </div>
                    <div class="col-3 text-black">
                        <h5 class="mb-5">ON SALE</h5>
                        <div class="cards d-flex justify-content-between mb-2">
                            <div class="description">
                                <h6>
                                    Black Leather Jacket
                                </h6>
                                <div class="stars">
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                </div>
                                <h6>
                                    $45
                                </h6>
                            </div>
                            <div class="poster">
                                <img src="../assets/images/black_elegant_leather_jacket-120x156.jpg" alt="">
                            </div>
                        </div>
                        <hr>
                        <div class="cards d-flex justify-content-between mb-2">
                            <div class="description">
                                <h6>
                                    Blue Leather Jacket
                                </h6>
                                <h6>
                                    $60
                                </h6>
                            </div>
                            <div class="poster">
                                <img src="../assets/images/blue_leather_jacket-120x156.jpg" alt="">
                            </div>
                        </div>
                        <hr>
                        <div class="cards d-flex justify-content-between">
                            <div class="description">
                                <h6>
                                    Modern Leather Boots
                                </h6>
                                <h6>
                                    $30
                                </h6>
                            </div>
                            <div class="poster">
                                <img src="../assets/images/modern_leather_boots-120x156.jpg" alt="">
                            </div>
                        </div>
                        <hr>
                    </div>
                    <div class="col-3 text-black">
                        <h5 class="mb-5">TOP RATED</h5>
                        <div class="cards d-flex justify-content-between mb-2">
                            <div class="description">
                                <h6>
                                    Leather Gloves
                                </h6>
                                <div class="stars">
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                </div>
                                <h6>
                                    $45
                                </h6>
                            </div>
                            <div class="poster">
                                <img src="../assets/images/leather_gloves-120x156.jpg" alt="">
                            </div>
                        </div>
                        <hr>
                        <div class="cards d-flex justify-content-between mb-2">
                            <div class="description">
                                <h6>
                                    Black Leather Jacket
                                </h6>
                                <div class="stars">
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                </div>
                                <h6>
                                    $200
                                </h6>
                            </div>
                            <div class="poster">
                                <img src="../assets/images/black_elegant_leather_jacket-120x156.jpg" alt="">
                            </div>
                        </div>
                        <hr>
                        <div class="cards d-flex justify-content-between">
                            <div class="description">
                                <h6>
                                    Spring Printed Dress
                                </h6>
                                <div class="stars">
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                </div>
                                <h6>
                                    $47
                                </h6>
                            </div>
                            <div class="poster">
                                <img src="../assets/images/spring_printed_dress-120x156.jpg" alt="">
                            </div>
                        </div>
                        <hr>
                    </div>
                    <div class="col-3 text-black">
                        <h5 class="mb-5">LATEST REVIEWS</h5>
                        <div class="cards d-flex justify-content-between mb-2">
                            <div class="description">
                                <h6>
                                    Leather Gloves
                                </h6>
                                <div class="stars">
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                </div>
                                <h6>
                                    by Admin
                                </h6>
                            </div>
                            <div class="poster">
                                <img src="../assets/images/leather_gloves-120x156.jpg" alt="">
                            </div>
                        </div>
                        <hr>
                        <div class="cards d-flex justify-content-between mb-2">
                            <div class="description">
                                <h6>
                                    Black Leather Jacket
                                </h6>
                                <div class="stars">
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                </div>
                                <h6>
                                    by Admin
                                </h6>
                            </div>
                            <div class="poster">
                                <img src="../assets/images/black_elegant_leather_jacket-120x156.jpg" alt="">
                            </div>
                        </div>
                        <hr>
                        <div class="cards d-flex justify-content-between">
                            <div class="description">
                                <h6>
                                    Spring Printed Dress
                                </h6>
                                <div class="stars">
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                    <i class="fa-solid fa-star" style="color: #417ac8;"></i>
                                </div>
                                <h6>
                                    by Admin
                                </h6>
                            </div>
                            <div class="poster">
                                <img src="../assets/images/spring_printed_dress-120x156.jpg" alt="">
                            </div>
                        </div>
                        <hr>
                    </div>
                </div>
            </div>

        </section>
        
        
    </main>
</template>

<style lang="scss" scoped>
@use "../assets/scss/partials/variables.scss" as *;
    main {
        overflow-x: hidden;
    }
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

    .button:hover{
        text-decoration: none;
        background-color: white;
        border-radius: 30px;
        padding: 20px 30px;
        border: 1px solid white;
        color: white;
        font-size: 1rem;
        font-weight: 400;
        color: black;
        font-weight: bold;

    }
    .jumbo {
        background-image: url(../assets/images/home1_slide_three_bg_2.jpg);
        background-size: cover;
        height: 500px;
    }

    h3 {
        font-size: 50px;
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
                    bottom: 100px;
                    left: 50%;
                    margin-left: -125px;
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
                    bottom: 100px;
                    left: 50%;
                    margin-left: -125px;
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
                    bottom: 100px;
                    left: 50%;
                    margin-left: -125px;
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
            width: 30px;
            height: 40px;
            margin: 10px 0;
            background: #4b78c6;
            cursor: pointer;
            color: white;
            border: none;
        }
        .prev-btn {
            position: absolute;
            left: 20px;
            top: 50%;
            margin-top: -20px;
        }
        .next-btn {
            position: absolute;
            right: 20px;
            top: 50%;
            margin-top: -20px;
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

    .new-arrivals {
        .slider-wrapper {
            position: relative;
        }
        h3 {
            font-weight: bold;
        }
        .prev-btn, .next-btn {
            width: 40px;
            height: 60px;
            margin: 10px 0;
            background: #4b78c6;
            cursor: pointer;
            color: white;
            border: none;
        }
        .prev-btn {
            position: absolute;
            left: 20px;
            top: 50%;
            margin-top: -30px;
        }
        .next-btn {
            position: absolute;
            right: 20px;
            top: 50%;
            margin-top: -30px;
        }
    }

    .testimonial {
        height: 500px;
        background-image: url(../assets/images/testimonials_home_1_bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        .wrapper {
            text-align: center;
            max-width: 800px;
            color: white;
            p {
                margin: 30px 0;
            }
            i {
                font-size: 8px;
                margin: 0 5px;
            }
            .circle-container {
                display: flex;
                justify-content: center;
                align-items: center;
                margin-top: 10px;
            }

            .circle {
                display: block;
                width: 16px;
                height: 16px;
                border-radius: 50%;
                background-color: transparent;
                border: 1px solid white;
                margin: 0 10px;
                margin-top: 10px;
                cursor: pointer;
            }

            .circle.active {
                background-color: #428cdd;
            }
        }
    }

    .blog {
        .container {
            margin-bottom: 50px;
        }
        h3 {
            font-weight: bold;
        }
        .container {
            h6 {
                font-size: 22px;
                font-weight: bold;
            }
        }
    }

    .suggested-product {
        padding: 80px;
    }



</style>