<template>
    <v-sheet
    class="hero-container"
    height="100vh"
    width="100vw"
    color="#01497c"
    >
        <div class="about">
            <h1 class="animate__animated animate__pulse">Jackie Nguy</h1>
            <h1 class="title_text">Web Developer</h1>
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
// Google font style import
@import url('https://fonts.googleapis.com/css2?family=Lobster+Two:ital@1&display=swap');

.hero-container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(2, 1fr);
    overflow-x: none;
}

.about {
    margin: 0 30vw;
    text-align: center;
    padding-top: 30vh;
    grid-column: 1/4;

    
}

.resume_btn {
    margin-top: 20px;
    grid-column: 2/3;
    grid-row: 2/3;
    text-align: center;
}

.animate__animated {
    font-size: 4.5rem;
    font-family: 'Lobster Two', cursive;
    color: #ffd60a;
}

.title_text {
    color: #ffd60a;
}

// Small screen
@media screen and (max-width: 960px) {
    .animate__animated {
        font-size: 3rem;
    }

    .about {
        padding-top: 20vh;
    }
}



</style>