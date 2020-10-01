<template>
    <div>
        <section class="nav-block">
            <MainNav/>
        </section>
        <section class="pricing-header">
            <div class="pricing-header-container">
                <h1>Pricing</h1>
                <p>Whether you're a hobbyist or global superstar, Tidze has a plan to help you grow and earn money through live streaming.</p>
            </div>
        </section>
        <section class="pricing-content">

            <img src="@/assets/images/shape-mission.svg" class="shape-mission">

            <div class="pricing-content-container">
                <div class="plan-content">
                    <h2>Starter</h2>
                    <p style="padding-bottom: 19px">No contracts or monthly fees, only pay when you sell a ticket.</p>
                    <h3>
                        <span class="currency">€</span>
                        <span class="cost">0</span>
                        <br>
                        <span class="additional-info">per month</span>
                    </h3>
                    <div class="booking-fee-info">
                        <p>5% booking fee*</p>
                    </div>

                    <a class="butt-primary">Create my channel</a>

                    <div class="advantages-info-block">
                        <h4>Includes:</h4>
                        <ul class="advantages-info-list">
                            <li>Unlimited live streams</li>
                            <li>1 hour per live stream</li>
                            <li>Your own branded channel</li>
                            <li>Live broadcast to unlimited viewers</li>
                            <li>Live stream (like Zoom) with 200 participants</li>
                            <li>Max 720p video</li>
                            <li>'Powered By Tidze' branding</li>
                            <li>Email support</li>
                        </ul>
                    </div>
                </div>

                <div class="plan-content">
                    <div class="popular-content">
                        <p>Recommends</p>
                    </div>
                    <h2>Plus</h2>
                    <p>Longer live streams and reduced booking fees to help grow your business.</p>
                    <h3>
                        <span class="currency">€</span>
                        <span class="cost">59</span>
                        <br>
                        <span class="additional-info">per month</span>
                    </h3>
                    <div class="booking-fee-info">
                        <p>3% booking fee*</p>
                    </div>

                    <a class="butt-primary">Create my channel</a> 

                    <div class="advantages-info-block">
                        <h4>Includes:</h4>
                        <ul class="advantages-info-list">
                            <li>Unlimited live streams</li>
                            <li>2 hour per live stream</li>
                            <li>Your own branded channel</li>
                            <li>Live broadcast to unlimited viewers</li>
                            <li>Live stream (like Zoom) with 200 participants</li>
                            <li>Max 720p video</li>
                            <li>'Powered By Tidze' branding</li>
                            <li>Email and live chat support</li>
                        </ul>
                    </div>
                </div>

                <div class="plan-content">
                    <h2>Professional</h2>
                    <p>For pros that want to go fully branded and build a successful live streaming channel.</p>
                    <h3>
                        <span class="currency">€</span>
                        <span class="cost">109</span>
                        <br>
                        <span class="additional-info">per month</span>
                    </h3>
                    <div class="booking-fee-info">
                        <p>2% booking fee*</p>
                    </div>

                    <a class="butt-primary">Create my channel</a>

                    <div class="advantages-info-block">
                        <h4>Includes</h4>
                        <ul class="advantages-info-list">
                            <li>Unlimited live streams</li>
                            <li>4 hour per live stream</li>
                            <li>Your own branded channel</li>
                            <li>Live broadcast to unlimited viewers</li>
                            <li>Live stream (like Zoom) with 200 participants</li>
                            <li>Max 1080p video</li>
                            <li>No 'Powered By Tidze' branding</li>
                            <li>High priority email and live chat support</li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>
        <section class="pricing-notice">
            <div class="pricing-notice-container">
                <p>* a minimum booking fee of <span class="currency">€</span>0.60 (including sales tax) is charged per ticket sold.
                <br>
                All monthly subscription plans include sales tax (or VAT).</p>
            </div>
        </section>

        <section class="pricing-helper">
            <img src="@/assets/images/shape-what-is-tidze.svg" class="shape">

            <div class="pricing-helper-container">
                <div class="left-side-block">
                    <h2>Frequently asked pricing questions</h2>
                    <p>
                        Haven’t found what you’re looking for?
                        <br>
                        Take a look at our FAQs page
                    </p>
                </div>

                <div class="right-slide-block-pricing-page">
                    <h3>Do you offer a free trial?</h3>
                    <div>
                        <p>We don't offer a free trial as such. However, you can use the 'Starter' plan and pay no monthly fee.</p>
                        <p>The starter plan includes all the core features to earn money through live streaming. 
                            Move onto the Plus or Professional plan when you want to stream for longer or to reduce the booking fee.
                        </p>
                    </div>
                    <h3>Can I pay the monthly fee by other payment methods?</h3>
                    <div>
                        <p>Certainly! Whilst we encourage you to pay and mange your subscription with a debit/credit card we understand this doesn't work for everyone.</p>
                        <p>Please contact the billing team to discuss an alternative payment method - billing@tidze.com</p>
                    </div>
                    <h3>Does the Tidze booking fee include payment processing fees?</h3>
                    <div>
                        <p>The Tidze booking fee does not include payment processing fees. We've partnered with Stripe to allow you to take online payments.</p>
                        <p>All online payments will incur a Stripe processing fee, currently 1.4% + 20p for UK and EU cards and 2.9% + 20p for the rest of the world.</p>
                        <p>Please check with Stripe to confirm the processing fee for your region. They may be able to offer discounts for charities or high volume customers.</p>
                    </div>
                </div>
            </div>
        </section>

        <Footer/>
    </div>    
</template>

<script>
import MainNav from './main-nav-part'
import Footer from './footer-part'

export default {
    components: {
        MainNav,
        Footer
    },
    mounted: function() {
        let questionsBlock = document.getElementsByClassName('right-slide-block-pricing-page')[0]
        let questionsHeader = questionsBlock.getElementsByTagName('h3')
        let questionsContent = questionsBlock.getElementsByTagName('div')

        for (let i = 0; i < questionsHeader.length; i++) {
            questionsHeader[i].addEventListener('click', function(event) {
                console.log('qa')
                questionsHeader[i].classList.toggle('background-img-minus')
                questionsContent[i].classList.toggle('show')
            })
        }
    }
}

</script>

<style lang="scss">

.nav-block {
  height: 10vh;

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
/* .footer {

    .footer-container {
        min-width: 1156px;
        padding: 0 22px;
    }
} */
</style>

<style lang="scss" scoped>
@import '@/assets/styles/global.scss';

.show {
    /* display: block !important; */
    height: 150px !important;
    opacity: 1 !important;
    @media (max-width: 450px) {
        height: 250px !important;
    }
    @media (max-width: 300px) {
        height: 400px !important;
    }
}

.background-img-minus {
    &::before {background: #f6f7fb url('../assets/images/icon-minus.png') no-repeat 50% !important;}
}

.pricing-header {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    min-height: 200px;
    margin-top: calc(1.75rem + 1vw);

        .pricing-header-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            max-width: 760px;
            padding: 0 20px;

                h1 {
                    font-size: calc(1.5375rem + 3.45vw);
                    color: $main-color;
                    margin: 0;
                }
                p {
                    font-family: $text-bold-font;
                    text-align: center;
                    color: $main-color;
                    font-size: calc(1.275rem + .3vw);
                    opacity: 0.7;
                }
        }
}

.pricing-content {
    display: flex;
    justify-content: center;
    position: relative;
    width: 100%;

    .shape-mission {
        position: absolute;
        left: 0;
        top: 40%;
    }

    .pricing-content-container {
        display: flex;
        justify-content: space-around;
        margin-top: calc(2rem + 2vw);
        max-width: 1156px;
        padding: 0 22px;
        z-index: 10;

            .plan-content:nth-child(1) { 
                margin-right: calc(1.375rem + 1.5vw);
            } 
            .plan-content:nth-child(2) {
                position: relative;
                border: 1px rgb(255,185,162) solid;

                .popular-content {
                    position: absolute;
                    top: -28px;
                    width: calc(96% + 2px);
                    padding: 6px;
                    border: 1px rgb(255,185,162) solid;
                    border-top-left-radius: 6px;
                    border-top-right-radius: 6px;
                    background-color: rgb(255,185,162);

                    p {
                        font-family: $header-font;
                        margin: 0;
                        color: $main-color;
                        font-size: 14px;
                        opacity: 1;
                    }
                }
            }
            .plan-content:nth-child(3) { 
                margin-left: calc(1.375rem + 1.5vw);
            } 

            .plan-content:hover {
                cursor: pointer;
                transform: scale(1.02);
            }

            .plan-content {
                display: flex;
                flex-direction: column;
                align-items: center;
                min-height: 700px;
                max-width: calc(250px + 2vw);
                padding: 45px 30px;
                border: 1px rgb(230,231,253) solid;
                border-radius: 7px;
                background-color: #FFF;

                transition: all 200ms ease-out;
                
                .butt-primary {
                        font-family: $text-font;
                        width: 100%;
                        height: 60px;
                        margin-top: 45px;
                        border-radius: 10px;
                        text-align: center;
                        line-height: 60px;

                        transition: background-color 300ms;
                        color: $main-color;
                        border: 1px $main-color solid;
                    }

                .butt-primary:hover {
                    cursor: pointer;
                    color: white;
                    background-color: $main-color;
                }

                h2 {
                    font-family: $header-font;
                    color: $main-color;
                }
                h3 {
                    text-align: center;
                }
                .currency {
                    font-family: $text-bold-font;
                    font-size: calc(1.3125rem + .75vw);
                    opacity: 0.8;
                }
                .cost {
                    font-family: $text-bold-font;
                    color: $main-color;
                    font-size: calc(1.5rem + 1.5vw);
                }
                .additional-info {
                    font-family: $text-font;
                    font-size: 14px;
                    opacity: 0.4;
                }
                p {
                    font-family: $text-font;
                    font-size: 14px;
                    color: $main-color;
                    text-align: center;
                    opacity: 0.5;
                }
                .booking-fee-info {
                    width: 100%;
                    border-top: 4px rgb(242,242,242) solid;
                    border-bottom: 4px rgb(242,242,242) solid;
                }
                .advantages-info-block {
                    margin-top: 25px;

                    h4 {
                        font-family: $text-font;
                        font-size: 14px;
                        color: $main-color;
                        opacity: 0.7;
                    }
                    ul {
                        padding: 0 0 0 18px;

                        li {
                            font-family: $text-font;
                            font-size: 14px;
                            color: $main-color;
                            opacity: 0.7;
                            margin-bottom: 10px;
                        }
                    }
                }
            }
    }
}

.pricing-notice {
    width: 100%;
    max-height: 120px;

    .pricing-notice-container {
        display: flex;
        justify-content: center;
        align-items: center;
        padding: 40px;

        p {
            font-family: $text-font;
            font-size: 14px;
            color: $main-color;
            text-align: center;
            opacity: 0.6;
        }
    }
}

.pricing-helper {
    position: relative;
    margin: 150px 0 180px 0;

    .shape {
        position: absolute;
    }

    .pricing-helper-container {
        display: flex;
        justify-content: space-between;
        max-width: 1156px;
        padding: 0 22px;
        margin: 0 auto;

        h2, h3 {
            font-family: $header-font;
            color: $main-color;
        }
        p {
            font-family: $text-font;
            color: $main-color;
        }

        .left-side-block {
            max-width: 370px;
            z-index: 10;
        
            h2 {
                font-size: 2.75rem;
                margin-top: 0;
            }
            p {
                font-family: $text-font;
                font-size: 14px;
                opacity: 0.7;
            }
        }

        .right-slide-block-pricing-page {
            max-width: 660px;
            z-index: 10;

            h3 {
                font-family: $text-font;
                position: relative;
                font-size: 1.5rem;
                margin-top: 0;
                padding: 0 60px 0 0;
            }
            h3::after {
                content: '';
                display: block;
                margin-top: 20px;
                height: 4px;
                width: calc(100% + 60px);
                border-bottom: 4px rgb(242,242,242) solid;
            }
            h3::before {
                content: '';
                position: absolute;
                right: 0;
                padding: 20px;
                border-radius: 100%;
                background: #f6f7fb url('../assets/images/icon-plus.png') no-repeat 50%;
            }
            h3:hover {
                cursor: pointer;
            }
            p {
                opacity: 0.7;
            }
            div {
                /* display: none; */
                height: 0;
                opacity: 0;

                transition: all 300ms ease-out;
            }
        }
    }

}

</style>

<style lang="scss">
@media (max-width: 950px) {
    .pricing-helper-container {
        flex-direction: column;
        h3 {
            width: 100%;
        }
    }
}
@media (max-width: 900px) {
    .pricing-content-container {
        flex-wrap: wrap;

        .plan-content:nth-child(3) {
            max-width: initial !important;
            margin-top: 30px;
            margin-left: 0 !important;
        }
    }
}
@media (max-width: 735px) {
    .plan-content {
        max-width: initial !important;
        margin-top: 30px;
        margin-left: 0 !important;
        margin-right: 0 !important;
    }
    .plan-content:nth-child(2) {
        margin-top: 50px;
    }
}
</style>