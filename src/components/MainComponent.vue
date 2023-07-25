<script>
export default {
    name: "MainComponent",
    data() {
        return {

        }
    },
    methods: {

    }
}
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
            <div class="container mt-5 pb-5">
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

</style>