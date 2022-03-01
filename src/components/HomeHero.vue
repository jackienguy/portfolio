<template>
    <v-sheet
    class="hero-container"
    height="100vh"
    width="100vw"
    color="#dfe7fd"
    >
        <div class="about" color="#dfe7fd">
            <h1 class="animate__animated animate__pulse">Jackie Nguy</h1>
            <h1 class="animate__animated animate__pulse animate__delay-1s">Web Developer</h1>
        </div>
         <div class="resume_btn"><v-btn >Contact</v-btn></div>
    </v-sheet>
</template>

       

<script>
    export default {
        name: "HomeHero",
    }
</script>

<style lang="scss" scoped>

.hero-container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
      grid-template-rows: repeat(2, 1fr);
}

.about {
    margin: 0 30vw;
    text-align: center;
    padding-top: 30vh;
    grid-column: 2/3;
    
    
}

.resume_btn {
    margin-top: 30px;
    grid-column: 2/3;
    grid-row: 2/3;
    text-align: center;
}

.animate__animated {
  font-size: 2.5rem;

}

// Small screen
@media screen and (max-width: 700px) {
    .animate__animated {
        font-size: 1.7;
    }
}

</style>