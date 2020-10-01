<template>
  <div>
    <section class="main-header">
      <div class="main-header-container">

        <MainNav/>

        <div class="title-card">
          <h1>It's <span class="infinite-linear-gradient">your</span> stage.</h1>
          <p>Tidze enables you to host paid online live events for your performances, workshops and classes.</p>
          <router-link to="/register" class="register-butt-primary">Get Started</router-link>
        </div>

        <div class="shape-1"><img src="@/assets/images/shape-1.svg" class="shape-1"></div>
        <div class="shape-2"><img src="@/assets/images/shape-2.svg" class="shape-2" width="380px" height="127px"></div>
      </div>
    </section>
    <section class="use-cases">
      <div class="use-cases-container">
        <div class="use-case">
          <img src="https://static.tidze.com/site/home/use-singer.jpg" alt="singer" class="lazyload" data-src="singer">
          <h2>For <strong>musicians</strong> & DJs to perform to a global audience</h2>
        </div>
        <div class="use-case">
          <img src="https://static.tidze.com/site/home/use-creator.jpg" data-src="creater" class="lazyload" alt="creater">
          <h2>For <strong>creators</strong> to share your skills and passions</h2>
        </div>
        <div class="use-case">
          <img src="https://static.tidze.com/site/home/use-theatre.jpg" data-src="theatre" class="lazyload" alt="theatre">
          <h2>For <strong>theatres</strong> to broadcast live and recorded performances</h2>
        </div>
        <div class="use-case">
          <img src="https://static.tidze.com/site/home/use-yoga.jpg" data-src="yoga" class="lazyload" alt="yoga">
          <h2>For <strong>teachers</strong> to educate, nurture and inspire</h2>
        </div>
        <div class="use-case">
          <img src="https://static.tidze.com/site/home/use-entertainer.jpg" data-src="entertainer" class="lazyload" alt="entertainer">
          <h2>For <strong>entertainers</strong> to create memorable moments</h2>
        </div>
        <div class="content-nav-list">
          <div class="content-nav-list-container">
            <div class="content-nav-item">
              <span class="nav-name">Musicians & DJs</span>
              <span class="active-line"></span>
            </div>
            <div class="content-nav-item">
              <span class="nav-name">Creators</span>
              <span class="active-line"></span>
            </div>
            <div class="content-nav-item">
              <span class="nav-name">Theatres</span>
              <span class="active-line"></span>
            </div>
            <div class="content-nav-item">
              <span class="nav-name">Teachers</span>
              <span class="active-line"></span>
            </div>
            <div class="content-nav-item">
              <span class="nav-name">Entertainers</span>
              <span class="active-line"></span>
            </div>
            <a class="find-more-butt">
              <div>
                <strong>+ many</strong>
                outher uses
                <br>
                Find out more
              </div>
            </a>
          </div>
        </div>
      </div>
    </section>

    <section class="section-feature-1 section-feature">
      <div class="section-feature-container">
        <div class="one-side-block">
          <div class="content">
            <img src="@/assets/images/section-feature-1/icons-business.svg">
            <h2>Take control of your live events</h2>
            <p>Professionally broadcast your live events in full HD and to an unlimited global audience.</p>
            <p>Alternatively, level-up your Zoom classes and events with a fully brandable, secure and payment gated live streaming platform.</p>
          </div>

        </div>
        <div class="second-side-block">
          <img src="@/assets/images/section-feature-1/live-interactive-dark@2x.jpg" class="image-feature">
        </div>
      </div>
    </section>

    <section class="section-feature-2 section-feature">
      <div class="section-feature-container">
        <div class="second-side-block">
          <img src="@/assets/images/section-feature-2/ui-ticket@2x.png" class="image-feature">
        </div>

        <div class="one-side-block">
          <div class="content">
            <img src="@/assets/images/section-feature-2/icons-money.svg">
            <h2>Earn money selling digital tickets</h2>
            <p>Sell secure digital tickets or accept donations to access your live events and classes.</p>
            <p>Boost your income by choosing to pass on the Tidze booking fee to your customers.</p>
          </div>
        </div>
      </div>
    </section>

    <section class="section-feature-3 section-feature">
      <div class="section-feature-container">
        <div class="one-side-block">
          <div class="content animate__animated animate__bounceInLeft">
            <img src="@/assets/images/section-feature-3/icons-experience.svg">
            <h2>Grow your audience</h2>
            <p>Reach a global audience by live streaming your performances, events and classes.</p>
            <p>Tidze enables you to create a members community, with marketing tools to promote and automatically share events with your members.</p>
          </div>
        </div>

        <div class="second-side-block">
          <img src="@/assets/images/section-feature-3/card@2x.png" class="image-feature">
        </div>
      </div>
    </section>

    <section class="section-feature-4 section-feature">
      <div class="section-feature-container">
        <div class="second-side-block">
          <img src="@/assets/images/section-feature-4/branded-channel@2x.jpg" class="image-feature">
        </div>

        <div class="one-side-block">
          <div class="content">
            <img src="@/assets/images/section-feature-4/icons-brand.svg">
            <h2>Create a branded website</h2>
            <p>Create your own stunning website to host and promote you live events and classes.</p>
            <p>Customise with your own colours, logos and images to bring your live streams on brand.</p>
          </div>
        </div>
      </div>
    </section>

    <section class="section-feature-5 section-feature">
      <div class="section-feature-container">
        <div class="one-side-block">
          <div class="content">
            <img src="@/assets/images/section-feature-5/icons-manage.svg">
            <h2>Manage your live events</h2>
            <p>Easily create and schedule unlimited live events across different time zones.</p>
            <p>Create engaging registration pages and waiting lists with your own content and images.</p>
          </div>

        </div>
        <div class="second-side-block">
          <img src="@/assets/images/section-feature-5/live-streams@2x.jpg" class="image-feature">
        </div>
      </div>
    </section>

    <section class="steps-slide">

      <h2>How to get started</h2>

      <div class="steps-slide-container">
        <div class="wrapper">
          <div class="step-slide"><img src="@/assets/images/steps-slide/step-1.png"></div>
          <div class="step-slide"><img src="@/assets/images/steps-slide/step-2.png"></div>
          <div class="step-slide"><img src="@/assets/images/steps-slide/step-3.png"></div>
          <div class="step-slide"><img src="@/assets/images/steps-slide/step-4.png"></div>
        </div>
      </div>

      <nav class="steps-nav">
        <div class="step-nav">  
          <div class="step-num">Step 1</div>
          <h3 class="step-name">Create a channel</h3>
        </div>
        <div class="step-nav">
          <div class="step-num">Step 2</div>
          <h3 class="step-name">Schedule a live stream</h3>
        </div>
        <div class="step-nav">
          <div class="step-num">Step 3</div>
          <h3 class="step-name">Host your live stream</h3>
        </div>
        <div class="step-nav">
          <div class="step-num">Step 4</div>
          <h3 class="step-name">Get paid</h3>
        </div>
      </nav>

    </section>

    <FooterAction/>
    <Footer></Footer>

  </div>
</template>

<script>
import MainNav from '@/components/main-nav-part'
import FooterAction from './footer-action-part'
import Footer from './footer-part'

export default {
  components: {
    MainNav,
    FooterAction,
    Footer,
  },
  mounted: function() {
    slideUseCase();
    showElementsOnScroll();
    showStepSlideOnClick();

    function slideUseCase() {
      let useCases = document.getElementsByClassName('use-case');
      let navCases = document.getElementsByClassName('content-nav-item');
      let lines = document.getElementsByClassName('active-line');
      let navName = document.getElementsByClassName('nav-name');
      let i = 0;
      let lastIndex = useCases.length - 1;
      let idInterval

      customLoop();

      function customLoop() {
        
       /*  moveCase(); */

        /* function moveCase() { */
          
          if (i == useCases.length) i = 0;

          useCases[lastIndex].classList.remove('show');
          useCases[i].classList.add('show');

          navName[lastIndex].classList.remove('show');
          navName[i].classList.add('show');

          lines[lastIndex].classList.remove('show-line');
          lines[i].classList.add('show-line');

          lastIndex = i;
          i++;
          idInterval = setTimeout(customLoop, 3500)
        /* } */
      }
      
      for (let j = 0; j < navCases.length; j++) {
        navCases[j].addEventListener('click', function() {
          clearTimeout(idInterval);
          i = j;
          customLoop();
        });
      }
  
    }

    function showElementsOnScroll() {
      let contentElements = document.getElementsByClassName('content')

      window.addEventListener('scroll', function() {
        for (let i = 0; i < contentElements.length; i++) {
          if (contentElements[i].getBoundingClientRect().top <= 800 && contentElements[i].getBoundingClientRect().bottom >= 60) {
            if (i % 2 == 0) {
              contentElements[i].classList.add('animate__animated');
              contentElements[i].classList.add('animate__bounceInLeft');
            }else {
              contentElements[i].classList.add('animate__animated');
              contentElements[i].classList.add('animate__bounceInRight');
            }
            
          }else {
            contentElements[i].classList.remove('animate__animated');
            contentElements[i].classList.remove('animate__bounceInLeft');
            contentElements[i].classList.remove('animate__bounceInRight');
          }
        }
        
      });
    }
    
    function showStepSlideOnClick() {
      let stepSlides = document.getElementsByClassName('step-slide');
      let stepNav = document.getElementsByClassName('step-nav');

      stepSlides[0].classList.add('show');
      stepNav[0].classList.add('show');
      stepNav[0].classList.add('showAfter');

      for (let i = 0; i < stepNav.length; i++) {
        stepNav[i].addEventListener('click', function() {
          for (let j = 0; j < stepNav.length; j++) {
            stepSlides[j].classList.remove('show');
            stepSlides[j].classList.remove('animate__animated');
            stepSlides[j].classList.remove('animate__backInUp');
            stepNav[j].classList.remove('show');
            stepNav[j].classList.remove('showAfter');
          }
          stepSlides[i].classList.add('show');
          stepSlides[i].classList.add('animate__animated');
          stepSlides[i].classList.add('animate__backInUp');
          stepNav[i].classList.add('show');
          stepNav[i].classList.add('showAfter');
        });
      }
    }

  }
}
</script>

<style lang="scss" scoped>
@import '@/assets/styles/global.scss';

.show {
    opacity: 1 !important;
}
.showAfter {
  &::after {
    content: '';
    position: absolute;
    top: -23px;
    width: 100%;
    max-width: 270px;
    height: 5px;
    border-radius: 5px;
    background-color: rgb(128,134,243);
  }
}

.show-line {
  width: 150px !important;
  visibility: visible !important;
}

%section-feature {
  width: 100%;
  height: 100vh;

  .section-feature-container {
    display: flex;
    width: 100%;
    height: 100%;

      .one-side-block {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        width: 50%;
        height: 100%;

        .content {
          margin: auto;
          max-width: 450px;
          color: $main-color;

          h2 {
            font-family: $header-font;
            text-align: left;
            font-size: calc(1.4rem + 1.8vw);
          }
          p {
            font-family: $text-font;
            opacity: .7;
          }
        }
      }

      .second-side-block {
        position: relative;
        width: 50%;
        height: 100%;
        background-repeat: no-repeat;
        background-size: 100% 100%;
      }
  }
}

%get-started-butt {
  /* font-family: $header-font; */
  margin-top: 25px;
  padding: 22px 35px;
  border-radius: 10px;

  transition: background-color 300ms;
}

  /* .infinite-linear-gradient {
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background: linear-gradient(-45deg, #ee7752, #e73c7e, #23a6d5, #23d5ab);
    background-size: 400% 400%;
    animation: gradient 15s ease infinite;

    @keyframes gradient {
      0% {
        background-position: 0% 50%;
      }
      50% {
        background-position: 100% 50%;
      }
      100% {
        background-position: 0% 50%;
      }
    }
  } */

  .main-header {
    position: relative;
    height: 100vh;
    width: 100%;
    background-color: rgb(24,39,67);

    a {
      text-decoration: none;
      color: white;
      font-size: 16px;
      font-family: $text-font;
    }
    a:hover {
      color: #8086f3;
    }

      .main-header-container {
        position: absolute;
        width: 100%;
        height: 100%;
        
        .title-card {
          display: flex;
          flex-direction: column;
          align-items: center;
          justify-content: center;
          margin: 0 auto;
          min-width: 40%;
          max-width: 65%;
          height: 80%;
          color: white;

            h1 {
              font-family: $header-font;
              font-size: calc(1.5rem + 4vw);
              margin-top: 0;
              margin-bottom: 10px;
              text-align: center;
              z-index: 100;
            }
            p {
              font-family: $text-bold-font;
              margin-top: 10px;
              font-size: calc(1rem + 1vw);
              text-align: center;
              z-index: 100;
            }
            .register-butt-primary {
              @extend %get-started-butt;
              background-color: #8086F3;

              transition: background-color 300ms;
            }
            .register-butt-primary:hover {
              color: white;
              cursor: pointer;
              background-color: #515AEF;
            }
        }

        .shape-1 {
          position: absolute;
          top: 35%;
          z-index: 10;
        }
        .shape-2 {
          position: absolute;
          width: 550px;
          right: 0;
          top: 0;
          z-index: 10;
        }
      }
  }

  .use-cases {
    position: relative;
    width: 100%;
    height: 100vh;

      .use-case {
        display: flex;
        justify-content: center;
        align-items: center;
        position: absolute;
        opacity: 0;

        transition: opacity 300ms ease-in;

          img {
            width: 100vw;
            height: 100vh;
          }
          h2 {
            position: absolute;
            max-width: 800px;
            font-family: $text-bold-font;
            font-size: calc(1.4rem + 1.8vw);
            text-align: center;
            color: #FFF;
            z-index: 10;
          }
      }

      .use-case:after {
        content: '';
        background: rgba(45,45,45,.4);
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        z-index: 2;
      }
      .content-nav-list {
        position: absolute;
        top: 70%;
        left: 50%;
        width: $main-width-content;
        transform: translateX(-50%);
        z-index: 10;

          .content-nav-list-container {
            display: flex;
            justify-content: space-between;
            align-items: flex-end;
            position: relative;
            margin: 0 auto;
            padding: 0 20px;
            max-width: calc(1200px - 40px);
            z-index: 10;

            .content-nav-item {
              display: flex;
              flex-direction: column;
              width: 100%;
              max-width: 150px;
              font-size: 20px;
              color: #FFF;
              z-index: 10;

                span {
                  opacity: 0.5;
                }
                span:hover {
                  opacity: 0.7;
                }
                .active-line {
                  position: absolute;
                  bottom: 0;
                  width: 0px;
                  height: 4px;
                  opacity: 1;
                  visibility: hidden;
                  background-color: #FFF;

                  transition: width 3500ms ease-out;
                }

            }
            .content-nav-item::after {
              content: '';
              margin-top: 5px;
              height: 4px;
              border-radius: 4px;
              opacity: 0.5;
              background-color: #FFF;
            }
            .content-nav-item:hover {
              cursor: pointer;
            }
          }
            .find-more-butt {
              display: flex;
              justify-content: center;
              align-items: center;
              font-family: $text-font;
              color: #FFFFFF;
              text-align: center;
              width: 166px;
              height: 142px;
              padding: 10px;
              border: 2px #FFF solid;
              border-radius: 10px;
              z-index: 10;
            }
            .find-more-butt:hover {
              cursor: pointer;
            }
      }
  }

  .section-feature-1 {
    @extend %section-feature;
    .second-side-block {
      background-image: url('../assets/images/section-feature-1/home-feature-2.jpg');

      img {
        position: absolute;
        top: 50%;
        right: 0;
        transform: translateY(-50%);
        max-width: 80%;
        }
    }
  }

  .section-feature-2 {
    @extend %section-feature;

      .second-side-block {
        background-image: url('../assets/images/section-feature-2/home-feature-3.jpg');
          img {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            max-width: 80%;
          }
      }

  }

  .section-feature-3 {
    @extend %section-feature;
    .second-side-block {
      background-image: url('../assets/images/section-feature-3/home-feature-1.jpg');

      img {
        position: absolute;
        top: 50%;
        right: 0;
        transform: translateY(-50%);
        max-width: 80%;
        }
    }
  }

  .section-feature-4 {
    @extend %section-feature;
    .second-side-block {
      background-image: url('../assets/images/section-feature-4/home-feature-4.jpg');

      img {
        position: absolute;
        top: 50%;
        right: 0;
        transform: translateY(-50%);
        max-width: 80%;
        }
    }
  }

  .section-feature-5 {
    @extend %section-feature;
    .second-side-block {
      background-image: url('../assets/images/section-feature-5/home-feature-5.jpg');

      img {
        position: absolute;
        top: 50%;
        right: 0;
        transform: translateY(-50%);
        max-width: 80%;
        }
    }
  }

  .steps-slide {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding-bottom: 150px;
    width: 100%;
    background-color: rgb(246,247,251);


      h2 {
        font-family: $header-font;
        text-align: left;
        color: $main-color;
        font-size: calc(1.4rem + 1.8vw);
      }

      .steps-slide-container {
        display: flex;
        flex-direction: column;
        justify-content: center;

        .wrapper {
          display: flex;
          align-items: center;
          max-height: 100%;
          min-height: 500px;
          width: $main-width-content;
          border-radius: 10px;
          background-color: rgb(190,220,209);

          .step-slide {
            display: flex;
            justify-content: center;
            align-items: center;
            width: calc(1200px - 40px);
            padding: 0 20px;

            img {
              max-width: 750px;
            }
          }
          .step-slide {
            position: absolute;
            opacity: 0;

            transition: opacity 300ms ease-out;
          }
        }
      }

      .steps-nav {
        display: flex;
        justify-content: space-between;
        position: relative;
        width: calc(1200px - 40px);
        margin-top: 40px;
        padding: 0 20px;

        .step-nav::before {
          content: '';
          position: absolute;
          top: -23px;
          width: 100%;
          max-width: 270px;
          height: 5px;
          border-radius: 5px;
          background-color: #e6e6e6;
        }

        .step-nav {
          width: 270px;
          max-width: 270px;
          opacity: 0.4;

          .step-num {
            font-family: $header-font;
            font-size: calc(1.275rem);
            text-align: center;
          }

          h3 {
            font-family: $text-font;
            font-size: calc(1.275rem + .3vw);
            margin-top: 5px;
            text-align: center;
          }
        }
        .step-nav:hover {
          cursor: pointer;
        }
      }
  }

</style>

<style lang="scss" scoped>
  @media (max-width: 1200px) {

    .content-nav-list {
      top: 40% !important;
      right: 0 !important;
      transform: translateX(0) !important;

      .content-nav-list-container {
      flex-direction: column;

      .content-nav-item {
        margin-bottom: 30px;
        }
      }
    }

    

    .steps-nav {
      width: calc(100vw - 40px) !important;
    }
  }

  @media (max-width: 800px) {
    .section-feature-1, .section-feature-3, .section-feature-5 {
      
      .section-feature-container {
        flex-direction: column;

        .one-side-block {
          width: 100%;
          padding: 60px 20px;
          
          img {
            @media (max-width: 500px) {
              transform: scale(.7);
            }
          }
        }
        .second-side-block {
          width: 100%;

          img {
            width: 35%;
            left: 50%;
          }
        }
      }
    }
    .section-feature-2, .section-feature-4 {

      .section-feature-container {
        flex-direction: column-reverse;

        .one-side-block {
          padding: 60px 20px;
          width: 100%;
          img {
            @media (max-width: 500px) {
              transform: scale(.7);
            }
          }
          
        }
        .second-side-block {
          width: 100%;

          img {
            width: 35%;
            left: 50%;
          }
        }
      }

    }
  }
</style>