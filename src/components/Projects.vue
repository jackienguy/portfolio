<template>
    <v-container>
        <v-row>
            <v-col cols="4" class="ml-12 mt-12">
                <h1>Projects</h1>
            </v-col>
        </v-row>

          <v-row class="projects-grid-container ">
   
                <div class="project-img1" data-aos="zoom-in" data-aos-duration="3000">
                   <v-img
                    src="https://images.unsplash.com/photo-1429216967620-ece20ff3a5f9?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHx0b3BpYy1mZWVkfDEwfDlRVlJFSDlBM0RVfHxlbnwwfHx8fA%3D%3D&auto=format&fit=crop&w=600&q=60"
                   ></v-img>
                </div>
                <div class="project-desc1" data-aos="zoom-in" data-aos-duration="3000">
                    <h3>Opt</h3>
                    <p><v-icon>fab fa-vuejs</v-icon></p>
                    <p>Minimum Viable Product (MVP) for my web development final project. Opt is a HCM platform for recruitment </p>
                    <v-btn>Live Site</v-btn> | <v-btn>Code</v-btn>
                   
                </div>

                 <div class="project-desc2" data-aos="zoom-in" data-aos-duration="3000">
                    <h3>Opt</h3>
                    <p><v-icon>fab fa-vuejs</v-icon></p>
                    <p>Minimum Viable Product (MVP) for my web development final project. Opt is a HCM platform for recruitment </p>
                    <v-btn>Live Site</v-btn> | <v-btn>Code</v-btn>
                </div>
                <div class="project-img2" data-aos="zoom-in" data-aos-duration="3000">
                   <v-img
                    src="https://images.unsplash.com/photo-1429216967620-ece20ff3a5f9?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHx0b3BpYy1mZWVkfDEwfDlRVlJFSDlBM0RVfHxlbnwwfHx8fA%3D%3D&auto=format&fit=crop&w=600&q=60"
                   ></v-img>
                </div>
               
         
        </v-row>

    </v-container>
</template>

<script>
    export default {
        name: "Projects"
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
   
}

.project-img1 {
    grid-column: 1 / 2;
    animation: fadeInTopLeft;
    animation-duration: 2s;
}

.project-desc1 {
    grid-column: 2 / 3;
}

.project-img2 {
    grid-column: 2 / 3;
}

.project-desc2 {
    grid-column: 1 / 2;
}

// Small screen 
@media screen and (max-width: 700px ) {
    .project-img1, .project-img2 {
        grid-column: 1 / 3;
    }

   .project-desc1, .project-desc2{
        grid-column: 1/ 3
    }

}

</style>