<template>
  <div id="app" class="bg-light">
    <app-nav-bar></app-nav-bar>
    <app-header></app-header>
    <app-skills></app-skills>
    <!--app-about></app-about>
    <app-projects></app-projects>
    <app-team></app-team-->
    <app-filler></app-filler>
    <!--app-customer></app-customer-->
    <app-blog></app-blog>
    <app-contact></app-contact>
    <app-review></app-review>
    <app-progress></app-progress>
    <app-price></app-price>
    <app-footer></app-footer>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Skills from './components/Skills.vue'
import About from './components/About.vue'
import Projects from './components/Projects.vue'
import Team from './components/Team.vue'
import Customer from './components/Customer.vue'
import Filler from './components/Filler.vue'
import Blog from './components/Blog.vue'
import Contact from './components/Contact.vue'
import Review from './components/Review.vue'
import Progress from './components/Progress.vue'
import Price from './components/Price.vue'
import Footer from './components/Footer.vue'
import NavBar from './components/NavBar.vue'


export default {
  name: 'App',
  components: {
    appHeader: Header,
    appCustomer: Customer,
    appSkills: Skills,
    appAbout: About,
    appProjects: Projects,
    appTeam: Team,
    appFiller: Filler,
    appBlog: Blog,
    appContact: Contact,
    appReview: Review,
    appProgress: Progress,
    appPrice: Price,
    appFooter: Footer,
    appNavBar: NavBar
  }
}
</script>

<style lang="scss">
  @import './styles/custom_bootstrap.scss';
  @import '../node_modules/bootstrap/scss/bootstrap.scss';
</style>

<style>
/*@import url('https://fonts.googleapis.com/css?family=Open+Sans|Permanent+Marker|Roboto');*/

body {
  margin-top: 60px;
}

.height-100 {
  min-height: 100vh;
}
.height-80 {
  min-height: 80vh;
}
.height-60 {
  min-height: 60vh;
}
.height-50 {
  min-height: 50vh;
}

.title-underline {
  height: 5px;
  margin: 0 auto;
  width: 100px;
}
</style>
