<template>
    <div>
        <section class="nav-block">
            <MainNav/>
        </section>

        <section class="about-header">

            <img src="@/assets/images/shape-mission-2.svg" class="shape-mission">

            <div class="about-header-container">
                <h1>Our Mission</h1>
                <p>
                    To empower creators, performers, musicians and teachers by providing a secure way to monetise 
                    their unique experiences and generate an income via an online live streaming platform.
                </p>
            </div>
            <div class="image-container">
                <div class="left-part"> 
                    <div class="img-1"></div>
                    <!-- <img src="@/assets/images/about-page/guitar.jpg" alt="A musician live streaming online" class="img-1"> -->
                    <img src="@/assets/images/about-page/img-2@2x.png" alt="A craft maker teaching an online class" class="img-2">
                </div>
                <div class="middle-part">
                    <img src="@/assets/images/about-page/img-1@2x.png" alt="A teacher teaching a child" class="img-3">
                </div>
                <div class="right-part">
                    <img src="@/assets/images/about-page/img-3@2x.png" alt="An artist painting to a live audience" class="img-4">
                    <img src="@/assets/images/about-page/img-4@2x.png" alt="A fitness instructor teaching a live online class" class="img-5">
                </div>
            </div>
        </section>

        <section class="what-is-tidze-block">

            <img src="@/assets/images/shape-what-is-tidze.svg">

            <div class="what-is-tidze-container">
                <div class="left-side">
                    <h2>What is Tidze?</h2>
                </div>

                <div class="right-side">
                    <p>Tidze is a UK-developed, all-in-one ticketing and live streaming platform, developed for the creative industries.</p>
                    <p>Share your expertise and generate income by creating a secure, fully branded online channel where performances, classes and events can be streamed live.</p>
                    <p>Earn money by selling tickets or accepting donations to access your live events and classes. Get started risk free, by using our Starter plan. You only pay a small booking fee each time you sell a ticket or accept a donation.</p>
                    <p>Built with funding from InnovateUK, the UK’s innovation agency, this is a platform that will revolutionise the creative industry whilst attending live events and classes is restricted, and will open up new audiences into the future.</p>
                </div>
            </div>
        </section>

        <section class="with-tidze-block">

            <h2>With Tidze, you can</h2>

            <div class="with-tidze-container">
                <div class="left-side">
                    <div class="feature">
                        <img src="@/assets/images/about-page/icon-create.svg">
                        <h3>Create</h3>
                        <p>Create your own beautifully crafted, fully branded channel</p>
                    </div>
                    <div class="feature">
                        <img src="@/assets/images/about-page/icon-sell.svg">
                        <h3>Sell</h3>
                        <p>Sell tickets or accept donations to access your live streams</p>
                    </div>
                    <div class="feature">
                        <img src="@/assets/images/about-page/icon-globe.svg">
                        <h3>Grow</h3>
                        <p>Grow your business and reach a global audience</p>
                    </div>
                </div>
                <div class="right-side">
                    <div class="feature">
                        <img src="@/assets/images/about-page/icon-manage.svg">
                        <h3>Manage</h3>
                        <p>Schedule and manage your live streaming activities</p>
                    </div>
                    <div class="feature">
                        <img src="@/assets/images/about-page/icon-stream.svg">
                        <h3>Stream</h3>
                        <p>Live stream 1:1, small groups (1:199) or broadcast 1:unlimited</p>
                    </div>
                </div>
            </div>
        </section>

        <FooterAction/>

        <Footer/>

    </div>
</template>

<script>
import MainNav from './main-nav-part'
import FooterAction from './footer-action-part'
import Footer from './footer-part'

export default {
    components: {
        MainNav,
        FooterAction,
        Footer
    }
}
</script>

<style lang="scss">

.nav-block {

  .nav-menu {
    margin: 0 auto;
    a {
      color: #182743;
    }
    a:hover {
      color: #8086F3;
    }
    a.register-butt {
      border: 1px #182343 solid;
    }
  }
}

</style>

<style lang="scss" scoped>
@import '@/assets/styles/global.scss';

    .about-header {
        display: flex;
        flex-direction: column;
        align-items: center;
        position: relative;
        width: 100%;
        min-height: 350px;

        .shape-mission {
            position: absolute;
            top: 53%;
            right: 0;
        }

        .about-header-container {
            max-width: 800px;
            z-index: 10;

            h1 {
                font-family: $header-font;
                font-size: 4.125rem;
                text-align: center;
                color: $main-color;
            }
            p {
                font-family: $text-bold-font;
                font-size: 1.5rem;
                text-align: center;
                color: $main-color;
                opacity: .7;
            }
        }

        .image-container {
            display: flex;
            position: relative;
            max-width: 1100px;
            margin: 0 auto;
            margin-top: 130px;
            z-index: 10;

            div {
                display: flex;
                flex-direction: column;
                position: relative;
                background-attachment: fixed;
            }
            
            .left-part {
                margin-right: 20px;
            }

            .middle-part {
                margin-right: 20px;
            }

            img, div {
                position: relative;
                border-radius: 10px;

                animation-name: float;
                animation-duration: 5s;
                animation-iteration-count: infinite;
                animation-timing-function: ease-out;
            }

            .img-1 {
                width: 374px;
                height: 250px;

                background: url('../assets/images/about-page/guitar.jpg') no-repeat;
                background-size: cover;
            }
            .img-2 {
                width: 170px;
                height: 115px;
                top: 30px;
                left: calc(374px - 170px);

            }
            .img-3 {
                width: 270px;
                height: 406px;
                bottom: 70px;
            }
            .img-4 {
                width: 170px;
                height: 115px;
            }
            .img-5 {
                width: 374px;
                height: 250px;
                top: 30px;
            }
        }
    }


@keyframes float {
    0% {
        transform: translateY(0);
    }
    50% {
        transform: translateY(-7px);
    }
    100% {
        transform: translateY(0);
    }
}

.what-is-tidze-block {
    display: flex;
    justify-content: center;
    position: relative;
    margin-top: calc(2.0625rem + 9.75vw);
    width: 100%;

    img {
        position: absolute;
        left: 0;
        top: 14%;
    }

    .what-is-tidze-container {
        display: flex;
        justify-content: space-between;
        width: 100%;
        max-width: 1160px;
        padding: 0 20px;
        z-index: 10;

        .left-side {

            h2 {
                font-family: $header-font;
                color: $main-color;
                font-size: 2.75rem;
                margin: 0;
            }
        }
        .right-side {
            display: flex;
            flex-direction: column;
            max-width: 600px;

            p {
                font-family: $text-bold-font;
                font-size: calc(1.275rem + .3vw);
                color: $main-color;
                margin: 0;
                opacity: .7;
            }
            p::after {
                content: '';
                display: block;
                height: 4px;
                width: 100%;
                margin: 40px 0;
                background: #f2f2f2;
            }
            p:last-child::after {
                display: none;
            }
        }
    }
}

.with-tidze-block {
    display: flex;
    flex-direction: column;
    margin: 10rem 0;
    width: 100%;

    h2 {
        font-family: $header-font;
        width: 1160px;
        margin: 0 auto;
        margin-bottom: 90px;
        padding: 0 20px;
        color: $main-color;
        font-size: 2.75rem;
    }

    .with-tidze-container {
        display: flex;
        justify-content: space-between;
        max-width: 1160px;
        padding: 0 20px;
        margin: 0 auto;
        z-index: 10;

        h3 {
            font-family: $header-font;
            color: $main-color;
            font-size: 1.5rem;
        }

        p {
            font-family: $text-bold-font;
            color: $main-color;
            font-size: 1.5rem;
            opacity: 0.7;
        }

        .left-side {
            max-width: 48%;
        }

        .right-side {
            max-width: 48%;
        }
    }
}

</style>

<style lang="scss">
@media (max-width: 950px) {
    .what-is-tidze-container {
        flex-direction: column;

        h2 {
            margin-bottom: 25px !important;
        }
    }
    .with-tidze-container {
        flex-direction: column;

        div {
            margin-bottom: 40px !important;
        }

        .left-side {
            max-width: initial !important;
        }
        .right-side {
            max-width: initial !important;
        }
    }
    .image-container {
        img, div {
            animation-name: floatX !important;
        }
    }
    @keyframes floatX {
        0% {
            transform: translateX(0);
        }
        50% {
            transform: translateX(-7px);
        }
        100% {
            transform: translateX(0);
        }
    }
}
</style>