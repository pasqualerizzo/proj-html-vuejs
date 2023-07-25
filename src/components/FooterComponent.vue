<script>
export default {
    name: "FooterComponent",
    data() {
        return {

        }
    },
    methods: {

    }
}
</script>

<template>
    <footer>
        <section class="partner">
            <h6 class="text-center pt-5">BRAND LOGOS</h6>
            <div class="container">
                <div class="row p-5">
                    <div class="col">
                        <img src="../assets/images/b_logotype_6.png" alt="">
                    </div>
                    <div class="col">
                        <img src="../assets/images/b_logotype_7.png" alt="">
                    </div>
                    <div class="col">
                        <img src="../assets/images/b_logotype_1.png" alt="">
                    </div>
                    <div class="col">
                        <img src="../assets/images/b_logotype_2.png" alt="">
                    </div>
                    <div class="col">
                        <img src="../assets/images/b_logotype_3.png" alt="">
                    </div>
                </div>
            </div>

        </section>
        <section class="newsletter-cta">
            <div class="container">
                <div class="row align-items-center">
                    <div class="col p-5 d-flex align-items-center">
                        <span>
                            <i class="fa-regular fa-envelope" style="color: #5b5d62;"></i>
                        </span>
                        <h3 class="m-0">
                            Subscribe now and get special offers
                        </h3>
                    </div>
                    <div class="col p-5 text-end">
                        <input type="search" name="email" id="" placeholder="Insert your email">
                        <button class="email-send">
                            SEND
                        </button>
                    </div>
                </div>
                
            </div>
        </section>
        <section class="footer-menu p-5">
            <div class="container">
                <div class="row">
                    <div class="col-3 info">
                        <img src="../assets/images/classic_shop_logo_footer.png" alt="">
                        <h6>
                            12345 North Main Street
                        </h6>
                        <h6>
                            New York. NY555555
                        </h6>
                        <h6>
                            Phone: 1.800.555.6789
                        </h6>
                        <h6>
                            Email: info@company.com
                        </h6>
                        <h6>
                            Web: Theme-company.com
                        </h6>
                        <div class="col-auto social">
                            <i class="fa-brands fa-facebook-f"></i>
                            <i class="fa-brands fa-twitter"></i>
                            <i class="fa-brands fa-instagram"></i>
                            <i class="fa-brands fa-youtube"></i>
                        </div>
                    </div>
                    <div class="col-3 text-white">
                        <h5 class="mb-3">TOP RATED PRODUCTS</h5>
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
                    <div class="col-3">
                        <h5 class="text-white mb-3">RECENT POST</h5>
                        <div class="post">
                            <i class="fa-solid fa-chevron-right" style="color: #e5e5e5;"></i>
                            <span class="text-white">
                                Lorem, ipsum dolor.
                            </span>
                            <hr>
                        </div>
                        <div class="post">
                            <i class="fa-solid fa-chevron-right" style="color: #e5e5e5;"></i>
                            <span class="text-white">
                                Lorem, ipsum dolor.
                            </span>
                            <hr>
                        </div>
                        <div class="post">
                            <i class="fa-solid fa-chevron-right" style="color: #e5e5e5;"></i>
                            <span class="text-white">
                                Lorem, ipsum dolor.
                            </span>
                            <hr>
                        </div>
                        <div class="post">
                            <i class="fa-solid fa-chevron-right" style="color: #e5e5e5;"></i>
                            <span class="text-white">
                                Lorem, ipsum dolor.
                            </span>
                            <hr>
                        </div>
                        <div class="post">
                            <i class="fa-solid fa-chevron-right" style="color: #e5e5e5;"></i>
                            <span class="text-white">
                                Lorem, ipsum dolor.
                            </span>
                            <hr>
                        </div>
                        <div class="post">
                            <i class="fa-solid fa-chevron-right" style="color: #e5e5e5;"></i>
                            <span class="text-white">
                                Lorem, ipsum dolor.
                            </span>
                            <hr>
                        </div>
                    </div>
                    <div class="col-3">
                        <h5 class="text-white mb-3">
                            TAGS
                        </h5>
                        <div class="wrapper-tag">
                            <span class="tag">tag</span>
                            <span class="tag">tag</span>
                            <span class="tag">tag</span>
                            <span class="tag">tag</span>
                            <span class="tag">tag</span>
                            <span class="tag">tag</span>
                            <span class="tag">tag</span>
                            <span class="tag">tag</span>
                            <span class="tag">tag</span>
                            <span class="tag">tag</span>
                            <span class="tag">tag</span>
                            <span class="tag">tag</span>
                            <span class="tag">tag</span>
                            <span class="tag">tag</span>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </footer>
</template>

<style lang="scss" scoped>
    .partner {
        background-color: #f6f6f6;
    }
    .newsletter-cta {
        background-color: #303337;
        span {
            background-color: #2b2e32;
            padding: 20px;
            border-radius: 50px;
            display: flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            margin-right: 10px;
        }
            span i {
                font-size: 1.5rem;
            }
        h3 {
            color: white;
            font-size: 1.2rem;
        }
        .row {

            input {
                border-radius: 30px;
                border: none;
                
            }
            input::placeholder {
                font-size: 12px;
                padding-left: 10px;
            }
            .email-send{
                padding: 2px 20px;
                border-radius: 50px;
                font-size: 0.8rem;
                color: white;
                background-color: #427ed1;
                border: none;
                margin-left: 10px;
            }
     }
    }
    .footer-menu {
        background-color: #2b2e32;
        display: flex;
        align-items: stretch;
        .info {
            img {
                height: 50px;
                margin-bottom: 40px;
            }
            h6 {
                color: white;
            }
            .social {
                color: white;
                margin-top: 40px;
                i {
                    margin-right: 10px;
                }
            }
        }
        h5 {
            margin-bottom: 20px;
        }
        .poster {
            height: 100%;
            img {
                height: 90px;
                border-radius: 10px;
            }
        }
        .stars {
            margin-bottom: 8px;
        }
        .post {
            i{
                font-size: 0.8rem,;
            }
            hr {
                color: white;
            }
        }
        .tag {
            color: white;
            border: 0.2px solid lightgray;
            background-color: transparent;
            padding: 5px 10px;
            font-size: 0.8rem;
        }
        .wrapper-tag {
            max-width: 100%;
            span {
                display: inline-block;
                margin-right: 5px;
            }
        }
    }
    h5 {
        font-size: 0.8rem;
    }
    h6 {
        font-size: 0.8rem;
    }
    span {
        font-size: 0.8rem;
    }

    
</style>