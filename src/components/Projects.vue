<template>
    <v-container>
        <v-row>
            <v-col cols="4" class="ml-12 mt-12">
                <h1>Projects</h1>
            </v-col>
        </v-row>

          <v-row class="projects-grid-container">
   
                <div class="project-img">
                   image goes here
                </div>
                <div class="project-desc">
                    <h3>Opt</h3>
                    <p>Minimum Viable Product (MVP) for my web development final project. Opt is a HCM platform for recruitment </p>
                    <p>Made with: <v-icon>fab fa-vuejs</v-icon></p>
                    <v-btn>Live Site</v-btn> | <v-btn>Code</v-btn>
                   
                </div>
         
        </v-row>

    </v-container>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>

.projects-grid-container {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: repeat(3, 1fr);
}

.projects-grid-container > div {
    padding: 20px;
    text-align: center;
    border: 2px black solid;
}

.project-img {
    grid-column: 1 / 2;
}

.project-desc {
     grid-column: 2 / 3;
}

</style>