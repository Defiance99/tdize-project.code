<template>
  <div>
    <section class="footer-action">
      <div class="footer-action-container">
        <div class="panel">
          <h2>Start your live streaming journey</h2>
          <p>Create your own branded channel and start earning money today.</p>
          <router-link to="/register" class="register-butt">Get Started</router-link>
        </div>
        <img src="@/assets/images/shape-3.svg" class="shape-3">
        <img src="@/assets/images/shape-4.svg" class="shape-4">
      </div>
    </section>
  </div>
</template>

<style lang="scss">
@import '@/assets/styles/global.scss';

%get-started-butt {
  /* font-family: $header-font; */
  font-family: $text-font;
  margin-top: 25px;
  padding: 22px 35px;
  border-radius: 10px;

  transition: background-color 300ms;
}

.footer-action {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 40vh;
    background-color: $main-color;

    .footer-action-container {
      display: flex;
      align-items: center;
      position: relative;
      width: $main-width-content;
      max-width: 1160px;
      max-height: 400px;
      padding: calc(1.6875rem + 5.25vw) 20px;
      border-radius: 15px;
      background-image: linear-gradient(90deg,#8086f3 0,#ffb9a2);

      .panel {
        display: flex;
        flex-direction: column;
        justify-content: center;
        max-width: 1160px;
        margin: 0 auto;
        z-index: 10;

        a {
          text-decoration: none;
        }

        h2 {
          font-family: $header-font;
          color: white;
          text-align: center;
          font-size: calc(1rem + 1.75vh);
          margin: 0;
        }
        p {
          font-family: $text-font;
          color: white;
          text-align: center;
          font-size: 16px;
        }
        .register-butt {
          @extend %get-started-butt;
          display: inline-block;
          text-align: center;
          margin: 20px auto;
          width: 100px;
          color: $main-color;
          background-color: #FFF;
        }
        .register-butt:hover {
          cursor: pointer;
          color: #FFF;
          background-color: $main-color;
        }
      }

      .shape-3 {
        position: absolute;
        left: 10px;
        top: 10px;
      }
      .shape-4 {
        position: absolute;
        right: 10px;
        bottom: 10px;
      }
    }
  }
</style>

<style lang="scss" scoped>

@media (max-height: 1600px) {
  .footer-action {
    height: 65vh;
  }
}


</style>