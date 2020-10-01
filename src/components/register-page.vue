<template>
  <div>
    <section class="register-block">
      <div class="register-block-container">
        <!-- <a href=""><img src="@/assets/images/brand-logo.png" width="120" height="55" alt="brand logo"></a> -->
        <a><router-link to="/" exact><img src="@/assets/images/brand-logo.png" alt="logo" width="120" height="55"></router-link></a>
        <div class="register-form">
          <h1>Create Your Free Account</h1>
          <label>Your email</label>
          <input 
            type="text" 
            v-model="email"
            @blur="$v.email.$touch()"
            v-bind:class="{invalidValue: $v.email.$error}"
          >
          <span class="error-required" v-if="$v.email.$error">- The 'email' field is required.</span>

          <label>Password</label>
          <input 
            type="text" 
            placeholder="5 characters or more" 
            v-model="password"
            @blur="$v.password.$touch()"
            v-bind:class="{invalidValue: $v.password.$error}"
          >
          <span class="error-required" v-if="$v.password.$error">- The 'password' field is required.</span>

          <label>Confrim password</label>
          <input 
            type="text" 
            v-model="repeatPassword"
            @blur="$v.repeatPassword.$touch()"
          >
          <span class="error-required" v-if="$v.repeatPassword.$error">- Passwords must be identical.</span>

          <input type="button" value="Create My Account" class="butt-primary">

          <p>By creating an account with Tidze, you agree to our Terms of Service and Privacy Policy.</p>
        </div>
        <p>© 2020 Tidze</p>
      </div>
    </section>
    <section class="image-block"></section>
  </div>
</template>

<script>
import { validationMixin } from 'vuelidate'
import { required, minLength, sameAs } from 'vuelidate/lib/validators'

export default {
  data() {
    return {
      email: '',
      password: '',
      repeatPassword: '',
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
    },
    repeatPassword: {
      sameAsPassword: sameAs('password')
    }
  },
}
</script>

<style lang="scss" scoped>
@import '@/assets/styles/global.scss';

%get-started-butt {
  font-family: $text-font;
  margin: 25px 0;
  padding: 10px 35px;
  border-radius: 6px;

  transition: background-color 300ms;
}

div:first-child {
  display: flex;
}

.register-block {
  display: flex;
  justify-content: center;
  width: 50vw;
  height: 100vh;
  background: #f6f7fb;

    .register-block-container {
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      height: 100%;

        img {
          margin: 15px 0;
        }

        img:hover {
          cursor: pointer;
        }

        .register-form {
          display: flex;
          flex-direction: column;
          max-width: 500px;

            h1, label {
              color: $main-color;
            }
            h1 {
              font-family: $header-font;
              font-size: 2.75rem;
              margin: 0 0 40px 0;
            }
            label {
              font-family: $text-font;
              margin: 0 0 10px 0;
            }
            p {
              font-family: $text-font;
              color: #7a818c;
            }
            input {
              font-size: 16px;
              padding: 10px;
              margin: 0 0 10px 0;
              color: $main-color;
              border-radius: 6px;
              border: 1px solid #d3d8eb;

              transition: border-color 200ms ease-out;
            }
            input:focus {
              border: 1px rgb(128,134,243) solid;
              outline: 0;
            }
            .butt-primary {
              @extend %get-started-butt;
              font-size: 16px;
              width: 100%;
              margin-top: 5px;
              max-width: 250px;
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
}

.image-block {
  width: 50vw;
  height: 100vh;
  background-image: url('../assets/images/register-page/female-DJ-759x600.jpg');
  background-size: cover;
  background-repeat: no-repeat;
}
</style>

<style lang="scss">
@media (max-width: 950px) {
  .register-block {
    width: 100% !important;
  }
  .image-block {
    display: none;
  }
}
</style>