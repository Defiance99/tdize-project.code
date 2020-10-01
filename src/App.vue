<template>
  <div id="app">
    <!-- <HomePage></HomePage> -->
    <!-- <LoginPage/> -->
    <!-- <RegisterPage/> -->
    <!-- <PricingPage/> -->
    <!-- <AboutPage/> -->
    <!-- <HelpPage/> -->
    <router-view></router-view>
  </div>
</template>

<script>
import VueRouter from 'vue-router'
import HomePage from '@/components/home-page.vue'
import LoginPage from '@/components/login-page.vue'
import RegisterPage from '@/components/register-page.vue'
import PricingPage from '@/components/pricing-page'
import AboutPage from '@/components/about-page'
import HelpPage from '@/components/help-page'

const routes = [
  {path: '/', component: HomePage},
  {path: '/login', component: LoginPage},
  {path: '/register', component: RegisterPage},
  {path: '/pricing', component: PricingPage},
  {path: '/about', component: AboutPage},
  {path: '/help', component: HelpPage},
]

const router = new VueRouter({
  /* mode: 'history', */
  routes: routes,
  base: '/defiance99.github.io/tdize-project.github.io/'
})

export default {
  name: 'App',
  components: {
    /* HomePage */
    /* LoginPage */
    /* RegisterPage */
    /* PricingPage */
    /* AboutPage */
    /* HelpPage */
  },
  router: router,
}
</script>

<style lang="scss">
  html,body {
    overflow-x: hidden;
    margin: 0;
    padding: 0;
  }
</style>
