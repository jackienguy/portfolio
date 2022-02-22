<template>
    <v-app>
      <v-main>
        <v-sheet
        class="hero-container"
        height="100vh"
        width="100vw"
        color="#dfe7fd"
        >
          <v-sheet class="about" color="#dfe7fd">
            <h1>Hi, I am Jackie</h1>
            <h1>Web Developer</h1>
            <p><v-btn>View Resume</v-btn></p>
          </v-sheet>
        </v-sheet>
        
        
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
import TopNav from '../components/TopNav.vue';
import Skills from '../components/Skills.vue';
import Projects from '../components/Projects.vue';
import Resume from '../components/Resume.vue';
import Contact from '../components/Contact.vue';
import Footer from '../components/Footer.vue';

export default {
  name: 'Home',
  components: { 
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

.about {
  margin: 0 30vw;
  text-align: center;
  padding-top: 35vh;
}


</style>
