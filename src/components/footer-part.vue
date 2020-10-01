<template>
    <div>
        <footer class="footer">
            <div class="footer-container">
                <div class="left-side-footer">
                    <a href="/"><img src="@/assets/images/brand-logo.png" alt="logo" width="150" height="50" class="logo-img"></a>
                    <p>© 2020 Tidze - Built in Lancashire - loved globally</p>
                </div>
                <div class="right-side-footer">
                    <router-link to="/pricing">Pricing</router-link>
                    <router-link to="/about">About</router-link>
                    <router-link to="/help">Help</router-link>
                    <router-link to="/login">Login</router-link>
                    <router-link to="/register">Get Started</router-link>
                </div>
            </div>
        </footer>
    </div>
</template>

<style lang="scss">
@import '@/assets/styles/global.scss';

%get-started-butt {
  font-family: $header-font;
  margin-top: 25px;
  padding: 22px 35px;
  border-radius: 10px;

  transition: background-color 300ms;
}

.footer {
    display: flex;
}

.footer {
    display: flex;
    justify-content: center;
    width: 100vw;
    height: 260px;
    background-color: $main-color;

    .footer-container {
      display: flex;
      justify-content: space-between;
      align-items: center;
      width: $main-width-content;

      .left-side-footer {
        a, p {
          font-family: $text-font;
          color: white;
        }
      }

      .right-side-footer {
        display: flex;
        flex-direction: column;

         a {
          font-family: $text-font;
          text-decoration: none;
          color: white;
          margin-top: 10px;
         }
         a:hover {
           color: #8086F3;
         }
      }
    }
}
</style>

<style lang="scss">
@media (max-width: 600px) {
  .footer {
    height: 300px;

    .footer-container {
      width: 90%;
      flex-direction: column-reverse;
      align-items: flex-start;
    
      .left-side-footer {
        padding-top: 30px;
      }
    }
  }
}
@media (max-width: 410px) {
  .footer {
    height: 350px;
  }
}
</style>