<template>
    <div>
        <section class="nav-block">
            <MainNav/>
        </section>

        <section class="help-header">
            <div class="help-header-container">
                <h1>Help</h1>
                <p>
                    We're here to help you to start earning money through live streaming.
                    <br>
                    If you don't find your answer below please contact support@tidze.com
                </p>
            </div>
        </section>

        <section class="help-block">
            <img src="@/assets/images/shape-what-is-tidze.svg" class="shape">

            <div class="help-container-one">
                <div class="left-side-block">
                    <h2>Using Tidze</h2>
                </div>

                <div class="right-slide-block">
                    <h3>What can I use Tidze for?</h3>
                    <div>
                        <p>Tidze is an all-in-one platform that allows you to sell digital tickets to access your live streams.</p>
                        <p>
                            You can use Tidze to run 1:1 sessions, interactive sessions with up to 200 participants (including yourself) or live broadcasts with an unlimited audience.
                        </p>
                    </div>
                    <h3>What's an interactive live stream?</h3>
                    <div>
                        <p>An interactive session is a lot like Zoom or Microsoft Teams.</p>
                        <p>As the host, you control the stage. You can mute everyone with one click!</p>
                        <p>An interactive live stream works directly from your web browser, there's no software or apps to install.</p>
                        <p>With an interactive live stream you can have up to 200 participants (including yourself).</p>
                    </div>
                    <h3>What's a live stream broadcast and how is it different to a live stream?</h3>
                    <div>
                        <p>
                            A live broadcast works in a similar way to platforms like Twitch: you're not able to view video feeds of the participants but they can see you. Live broadcasting is great if you want to reach a larger audience. There's no limit to the audience size, so it’s great for streaming concerts and theatre productions.
                        </p>
                        <p>
                            Our broadcasting supports 1080p HD video and is fully scalable and ready to support any event. Transmit your video feed by using an encoder that supports RTMP e.g. OBS
                        </p>
                    </div>
                    <h3>Do I need a good internet connection to live broadcast?</h3>
                    <div>
                        <p>The quality of the live broadcast and experience can be affected by your internet connection. We recommend connecting with an ethernet cable.</p>
                        <p>You will need a minimum upload speed of 2 Mbps, for higher quality video we would recommend a minimum upload speed of 5 Mbps.</p>
                    </div>
                    <h3>What are your recommended bitrates for live broadcasting?</h3>
                    <div>
                        <p>For 720p video at 30 frames per second, we recommend a bitrate of 1,500 to 3,000 kbps.</p>
                        <p>For 1080p video at 30 frames per second, we recommend a bitrate of 3,000 to 5,000 kbps.</p>
                    </div>
                </div>
            </div>

            <div class="help-container-second">
                <div class="left-side-block">
                    <h2>Payments</h2>
                </div>

                <div class="right-slide-block">
                    <h3>Do you offer a free trial?</h3>
                    <div>
                        <p>We don't offer a free trial. However, you can use the 'Starter' plan and pay no monthly fee.</p>
                        <p>
                            The starter plan includes all the core features to earn money through live streaming. Move onto the Professional plan when you want to stream for longer or to reduce the booking fee.
                        </p>
                    </div>
                    <h3>Can I pay the monthly fee by other payment methods?</h3>
                    <div>
                        <p>Certainly! Whilst we encourage you to pay and mange your subscription with a debit/credit card we understand this doesn't work for everyone.</p>
                        <p>Please contact the billing team to discuss an alternative payment method - billing@tidze.com</p>
                    </div>
                    <h3>Does the Tidze booking fee include payment processing fees?</h3>
                    <div>
                        <p>
                            The Tidze booking fee does not include payment processing fees. We've partnered with Stripe to allow you to take online payments.
                        </p>
                        <p>
                            All online payments will incur a Stripe processing fee, currently 1.4% + 20p for UK and EU cards and 2.9% + 20p for the rest of the world.
                        </p>
                        <p>
                            Please check with Stripe to confirm the processing fee for your region. They may be able to offer discounts for charities or high volume customers.
                        </p>
                    </div>
                    <h3>How do I switch to a different plan?</h3>
                    <div>
                        <p>You can switch to a new plan at any time by going to the Billing page in your dashboard.</p>
                        <p>Select the plan you’d like to switch to and immediately start using new features.</p>
                    </div>
                    <h3>Can I pass on the Tidze booking fee on to the customer?</h3>
                    <div>
                        <p>Yes! When creating a ticket you can choose to pass on the Tidze booking fee to the customer. This will add the booking fee on top of the ticket price.</p>
                    </div>
                    <h3>How long do payouts take?</h3>
                    <div>
                        <p>Payments will be made directly to your own Stripe account, they never touch our Tidze bank account. We recommend checking the Stripe documentation for their latest guidance on payouts.</p>
                    </div>
                    <h3>Can I pass on the Tidze booking fee on to the customer?</h3>
                    <div>
                        <p>Yes! When creating a ticket you can choose to pass on the Tidze booking fee to the customer. This will add the booking fee on top of the ticket price.</p>
                    </div>
                    <h3>Can I give refunds if my event is cancelled?</h3>
                    <div>
                        <p>Yes! Payments are made directly to your own Stripe account so simply refund the customer through this account. More information can be found here.</p>
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
    },
    mounted: function() {
        let questionsBlock = document.getElementsByClassName('right-slide-block')
        console.log('23')
        for (let i = 0; i < questionsBlock.length; i++) {
            let questionsHeader = questionsBlock[i].getElementsByTagName('h3')
            let questionsContent = questionsBlock[i].getElementsByTagName('div')

            for (let j = 0; j < questionsHeader.length; j++) {
                questionsHeader[j].addEventListener('click', function() {
                    console.log(questionsHeader)
                    questionsHeader[j].classList.toggle('background-img-minus')
                    questionsContent[j].classList.toggle('show')
                })
            }
        }
    }   
}

/* document.addEventListener('load', () => {
    
}); */

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
    height: 200px !important;
    opacity: 1 !important;
}

.background-img-minus {
    &::before {background: #f6f7fb url('../assets/images/icon-minus.png') no-repeat 50% !important;}
}

.help-header {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    min-height: 200px;
    margin-top: calc(1.75rem + 1vw);

        .help-header-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            max-width: 760px;
            padding: 0 20px;

                h1 {
                    font-family: $header-font;
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

.help-block {
    position: relative;
    margin: 150px 0 180px 0;

    .shape {
        position: absolute;
        top: 170px;
    }

    /* .help-container-second {
        margin-top: ;
    }
 */

    .help-container-second {
        margin-top: 5rem !important;
    }

    .help-container-one, .help-container-second {
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

        .right-slide-block {
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
                display: block;
                height: 0;
                opacity: 0;

                transition: all 300ms ease-out;
            }
        }
    }

}
</style>

<style lang="scss">
@media (max-width: 915px) {
    .help-container-one, .help-container-second {
        flex-direction: column;
    }
}
</style>