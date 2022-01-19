<template>
    <v-app>
      <v-main>
        <v-sheet
        height="100vh"
        width="100vw"
        class="blue text-center"
        >
          <div id="about" >
            <h1>Hi, I am Jackie</h1>
            <h1>Web Developer</h1>
          </div>
        </v-sheet>
        
        
        <!-- Top Navigation Bar -->
        <TopNav/>

        <Skills/> 
        <Projects/>
        <Resume/>
        <Contact/>  
      </v-main>
    </v-app>
</template>

<script>
import TopNav from '../components/TopNav.vue';
import Skills from '../components/Skills.vue';
import Projects from '../components/Projects.vue';
import Resume from '../components/Resume.vue';
import Contact from '../components/Contact.vue';

export default {
  name: 'Home',
  components: { 
    TopNav,
    Skills,
    Projects,
    Resume,
    Contact
  },
}
</script>

<style lang="scss" scoped>

</style>
