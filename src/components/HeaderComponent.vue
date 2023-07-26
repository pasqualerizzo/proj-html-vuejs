<script>
export default {
    name: "HeaderComponent",
    data() {
        return {

        }
    },
    methods: {

    }
}
</script>

<template>
    <header>
        <section class="header-top">
            <div class="container">
                <div class="row justify-content-between align-items-center">
                    <div class="col-auto social">
                        <i class="fa-brands fa-facebook-f"></i>
                        <i class="fa-brands fa-twitter"></i>
                        <i class="fa-brands fa-instagram"></i>
                        <i class="fa-brands fa-youtube"></i>
                    </div>
                    <div class="col-auto">
                        <nav class="navbar navbar-expand-lg p-0">
                            <div class="container">
                                
                                <div class="collapse navbar-collapse" id="navbarScroll">
                                    <ul class="navbar-nav me-auto my-2 my-lg-0 navbar-nav-scroll">
                                        <li class="nav-item shopping-cart p-2">
                                            <a class="nav-link active" aria-current="page" href="#">Shopping Cart</a>
                                        </li>
                                        <li class="nav-item dropdown my-account p-2">
                                            <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                                                My Account
                                            </a>
                                            <ul class="dropdown-menu">
                                                <li><a class="dropdown-item" href="#">Action</a></li>
                                                <li><a class="dropdown-item" href="#">Another action</a></li>
                                                <li><hr class="dropdown-divider"></li>
                                                <li><a class="dropdown-item" href="#">Something else here</a></li>
                                            </ul>
                                        </li>
                                        <li class="nav-item dropdown carrello">
                                            <i class="fa-solid fa-cart-shopping" style="color: #000000;"></i>
                                            <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                                                CART
                                            </a>
                                            <ul class="dropdown-menu">
                                                <li><a class="dropdown-item" href="#">Action</a></li>
                                                <li><a class="dropdown-item" href="#">Another action</a></li>
                                                <li><hr class="dropdown-divider"></li>
                                                <li><a class="dropdown-item" href="#">Something else here</a></li>
                                            </ul>
                                        </li>
                                    </ul>
                                </div>
                            </div>
                            </nav>
                    </div>
                </div>
            </div>
        </section>
        <section class="header-bottom">
            <div class="container">
                <div class="row justify-content-between align-items-center">
                    <div class="col-auto">
                        <div class="logo">
                            <img src="../assets/images/classic_shop_logo1x.png" alt="">
                        </div>
                    </div>
                    <div class="col-auto">
                        <nav class="navbar navbar-expand-lg">
                            <div class="container">
                                
                                <div class="collapse navbar-collapse" id="navbarScroll">
                                    <ul class="navbar-nav me-auto my-2 my-lg-0 navbar-nav-scroll">
                                        <li class="nav-item dropdown p-2">
                                            <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                                                Home
                                            </a>
                                            <ul class="dropdown-menu">
                                                <li><a class="dropdown-item" href="#">Action</a></li>
                                                <li><a class="dropdown-item" href="#">Another action</a></li>
                                                <li><hr class="dropdown-divider"></li>
                                                <li><a class="dropdown-item" href="#">Something else here</a></li>
                                            </ul>
                                        </li>
                                        <li class="nav-item dropdown p-2">
                                            <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                                                Shop
                                            </a>
                                            <ul class="dropdown-menu">
                                                <li><a class="dropdown-item" href="#">Action</a></li>
                                                <li><a class="dropdown-item" href="#">Another action</a></li>
                                                <li><hr class="dropdown-divider"></li>
                                                <li><a class="dropdown-item" href="#">Something else here</a></li>
                                            </ul>
                                        </li>
                                        <li class="nav-item dropdown p-2">
                                            <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                                                Products
                                            </a>
                                            <ul class="dropdown-menu">
                                                <li><a class="dropdown-item" href="#">Action</a></li>
                                                <li><a class="dropdown-item" href="#">Another action</a></li>
                                                <li><hr class="dropdown-divider"></li>
                                                <li><a class="dropdown-item" href="#">Something else here</a></li>
                                            </ul>
                                        </li>
                                        <li class="nav-item dropdown p-2">
                                            <a class="nav-link" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                                                News
                                            </a>
                                        </li>
                                        <li class="nav-item dropdown p-2">
                                            <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                                                Elements
                                            </a>
                                            <ul class="dropdown-menu">
                                                <li><a class="dropdown-item" href="#">Action</a></li>
                                                <li><a class="dropdown-item" href="#">Another action</a></li>
                                                <li><hr class="dropdown-divider"></li>
                                                <li><a class="dropdown-item" href="#">Something else here</a></li>
                                            </ul>
                                        </li>
                                    </ul>
                                    <a class="btn cta-shop" href="#" role="button">
                                            SHOP NOW!
                                    </a>
                                    <i class="fa-solid fa-magnifying-glass" style="color: #000000; cursor: pointer;"></i>
                                </div>
                            </div>
                            </nav>
                    </div>
                </div>
            </div>
        </section>
        
    </header>
</template>

<style lang="scss" scoped>

    .header-top {
        border: 1px solid lightgray;
    }
    .social {
        i {
            margin-right: 30px;
            font-size: 20px;
            color: #575c61;
            cursor: pointer;
        }
    }
    .shopping-cart, .my-account {
        border-right: 1px solid lightgray;
        a {
            color: black;
            display: inline-block;
        }
    }
    .carrello {
        padding: 0.5rem 80px;
        background-color: #fafafa;
        a{
            color: black;
            display: inline-block;
        }
    }


    .cta-shop {
        border-radius: 40px;
        background-color: #427ed1;
        color: white;
        font-weight: 600;
        font-size: 0.8rem;
        padding: 10px 20px;
        margin-right: 40px;
    }
    .cta-shop:hover {
        background-color: #427ed1;
        padding: 10px 30px;
        color: white;
        font-size: 1.2rem;
    }
</style>