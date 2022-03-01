<template>
    <v-app>
      <v-main>
        <!-- Hero Section -->
        <HomeHero/>
        
        <!-- Top Navigation Bar -->
        <TopNav/>

        <Skills/> 
        <Projects/>
        <Resume/>
        <Contact/>  
      </v-main>

      <v-footer>
        <Footer/>
      </v-footer>
    </v-app>
</template>

<script>
import HomeHero from '../components/HomeHero.vue';
import TopNav from '../components/TopNav.vue';
import Skills from '../components/Skills.vue';
import Projects from '../components/Projects.vue';
import Resume from '../components/Resume.vue';
import Contact from '../components/Contact.vue';
import Footer from '../components/Footer.vue';

export default {
  name: 'Home',
  components: { 
    HomeHero,
    TopNav,
    Skills,
    Projects,
    Resume,
    Contact,
    Footer
  },
}
</script>

<style lang="scss" scoped>

* {
  padding: 0px;
  margin: 0px;
}


</style>
