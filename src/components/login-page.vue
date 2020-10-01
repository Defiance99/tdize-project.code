<template>
  <div>
    <div class="nav-block">
      <MainNavPart/>
    </div>
    <section class="login-container">
      <div class="login-form">
        <label for="email">Email</label>
        <input 
          type="text" 
          class="typing-elem" 
          id="email" 
          v-model="email"
          @blur="$v.email.$touch()"
          v-bind:class="{invalidValue: $v.email.$error}"
        >
        <span class="error-required" v-if="$v.email.$error">- The 'Email' field is required.</span>

        <label for="password">Password</label>
        <input type="password" 
          class="typing-elem" 
          id="password" 
          v-model="password"
          @blur="$v.password.$touch()"
          v-bind:class="{invalidValue: $v.password.$error}"
        >
        <span class="error-required" v-if="$v.password.$error">- The 'Password' field is required.</span>

        <input type="button" value="Login" class="butt-primary">

        <div class="auth-links-container">
          <router-link to="/register" class="register-butt-primary">Register</router-link>
          <a href="/">Reset Password</a>
        </div>
      </div>
    </section>

    <Footer/>
    
  </div>
</template>

<script>
import { validationMixin } from 'vuelidate'
import { required, minLength } from 'vuelidate/lib/validators'
import MainNavPart from '@/components/main-nav-part'
import Footer from '@/components/footer-part.vue'

export default {
  data() {
    return {
      email: '',
      password: '',
    }
  },
  mixins: [validationMixin],
  validations: {
    email: {
      required,
      minLength: minLength(10)
    },
    password: {
      required,
      minLength: minLength(5)
    }
  },
  components: {
    MainNavPart,
    Footer
  }
}
</script>

<style lang="scss">

.error-required {
  color: red;
  margin-bottom: 5px;
}

.invalidValue {
  border: 1px red solid !important;
}

.nav-block {
  height: 10vh;
  background-color: #F6F7FB;

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
%get-started-butt {
  font-family: $header-font;
  margin: 25px 0;
  padding: 10px 35px;
  border-radius: 6px;

  transition: background-color 300ms;
}

  .login-container {
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: calc(90vh);
    background-color: #F6F7FB;

      .login-form {
        display: flex;
        flex-direction: column;
        min-width: 500px;
        height: 350px;
        padding: 30px;
        border: 1px rgb(221,221,221) solid;
        border-radius: 5px;
        box-shadow: 0 1px 3px 10px rgba(28,28,28,.014);
        background-color: #FFF;

        label {
          color: $main-color;
        }

        label {
          font-family: $text-font;
          margin: 0 0 10px 0;
        }

        .typing-elem {
          font-size: 16px;
          padding: 11px;
          margin: 0 0 10px 0;
          color: $main-color;
          border-radius: 6px;
          border: 1px solid #d3d8eb;

          transition: border-color 200ms ease-out;
        }
        .typing-elem:focus {
          border: 1px rgb(128,134,243) solid;
          outline: 0;
        }

        .auth-links-container {
          margin-top: 25px;

          a {
            font-family: $text-font;
            text-decoration: none;
            color: #7a818c;
          }
          a:first-child::after {
            content: '';
            margin: 0 7px;
            border-right: 1px #7a818c solid;
          }
          a:hover {
            cursor: pointer;
            color: #8086F3;
          }
        }

        .butt-primary {
          @extend %get-started-butt;
          font-size: 16px;
          max-width: 120px;
          height: 60px;
          border: 0;
          outline: 0;
          color: white;
          background-color: #8086F3;

          transition: background-color 300ms;
        }
        .butt-primary:hover {
          cursor: pointer;
          background-color: #515AEF;
        }
      }
  }

  .nav-menu {
    background-color: #F6F7FB !important;
  }
</style>
