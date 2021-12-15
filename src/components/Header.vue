<template>
    <header>
        <div class="container-nav-top">
            <div class="containerauto cont-nav">
                <ul class="nav-left stylenav">
                    <li>
                        <i class="fas fa-clock"></i> Open Hours: Mon - Sat - 9:00 - 18:00
                    </li>
                </ul>
                <ul class="nav-right stylenav">
                    <li>
                        <i class="fas fa-phone-alt"></i> +1 (305) 1234-5678
                    </li>
                    <li>
                        <i class="fas fa-envelope"></i> hello@exemple.com
                    </li>
                    <li>
                        <a href=""><i class="fab fa-facebook-f"></i></a>
                    </li>
                    <li>
                        <a href=""><i class="fab fa-twitter"></i></a>
                    </li>
                    <li>
                        <a href=""><i class="fab fa-linkedin-in"></i></a>
                    </li>
                </ul>
            </div>
        </div>
        <div class="jumbotron">
            <div class="containerauto">
                <nav class="nav-container">
                    <div class="logo-nexgen">
                        <img src="../assets/nexgen-logo.svg" alt="">
                    </div>
                    <ul class="navlist-style">
                        <li v-for="list, i in NavList" :key="i">
                            {{list}}
                        </li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>
</template>

<script>

export default {
  name: 'Header',
  props: {
        NavList: Array
    }
}
    
</script>

<style lang="scss">
    .container-nav-top {
        background-color: #21333e;
        height: 75px;
    }

    .cont-nav {
        width: 100%;
        height: 100%;
    }

    .containerauto {
        width: 70%;
        margin: 0 auto;
    }

    .nav-left {
        float: left;
    }

    .nav-right {
        float: right;
        justify-content: flex-end;
    }

    .stylenav {
        font-size: 17px;
        color: #c0c3d0;
        width: 50%;
        align-items: center;
        height: 100%;
        display: flex;
        flex-wrap: wrap;
        overflow: hidden;
        li {
            padding: 20px;
        }
    }

    .jumbotron {
        height: 1000px;
        width: 100%;
        background-image: url("../assets/bg-6.jpg");
    }

    .nav-container {
        height: 100px;
    }

    .logo-nexgen {
        display: flex;
        align-items: center;
        height: 100%;
        img {
            height: 75px;
        }
    }

    .navlist-style {
        display: flex;
        justify-content: flex-end;
        align-items: center;
        height: 100%;
        li {
            padding: 20px;
            cursor: pointer;
            color: #21333e;
        }
    }
</style>
