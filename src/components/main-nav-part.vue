<template>
  <div>
    <nav class="nav-menu">
      <div class="logo-block">
        <a><router-link to="/" exact><img src="@/assets/images/brand-logo.png" alt="logo" width="150" height="50" class="logo-img"></router-link></a>
      </div>
      <div class="elements-menu-block">
        <a><router-link to="/pricing">Pricing</router-link></a>
        <a><router-link to="/about" exact>About</router-link></a>
        <a><router-link to="/help" exact>Help</router-link></a>
      </div>
      <div class="auth-elements-block">
        <router-link to="/login" exact><a href="/login" class="login-butt">Login</a></router-link>
        <router-link to="/register" exact><a href="/register" class="register-butt">Get Started</a></router-link>
      </div>
    </nav>
  </div>
</template>

<style lang="scss">
@import '@/assets/styles/global.scss';

.nav-menu {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin: 20px auto;
  width: 95%;
  height: 80px;

  a {
    font-family: $text-font;
    text-decoration: none;
    color: white;
    font-size: 16px;
  }
  a:hover {
    color: #8086f3;
  }

    .logo-block {
      z-index: 100;

      .logo-img {
        border: 1px transparent solid;
        border-radius: 15px;
        transition: all 300ms;
      }
      .logo-img:hover {
        border: 1px white solid;
        background-color: white;
      }
    }

    .elements-menu-block {
      display: flex;
      justify-content: space-between;
      width: 210px;
      height: 22px;
      margin-left: 37.5px;
      z-index: 100;
    }

    .auth-elements-block {
      display: flex;
      justify-content: space-between;
      align-items: center;
      width: 200px;
      z-index: 100;

        .login-butt:hover {
          color: #FFB9A2;
        }

        .register-butt {
          /* font-family: $header-font; */
          padding: 5px 10px;
          border: 2px white solid;
          border-radius: 7px;

          transition: background-color 300ms ease-out;
        }
        .register-butt:hover {
          color: white;
          border: 2px $main-color solid;
          background-color: $main-color;
        }
    }
}
</style>

<style lang="scss" scoped>
@media (max-width: 750px) {
  .auth-elements-block, .elements-menu-block {
    display: none;
  }

  .auth-elements-block {
    background: url('../assets/images/mobile-icon-menu.jpg') no-repeat !important;
  }
}
</style>