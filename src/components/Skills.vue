<template>
    <v-container>
        <v-row>
            <v-col cols="4" md="8" class="ml-12 mt-12 mb-12">
                <h1>Skills and Competencies</h1>
            </v-col>
        </v-row>

        <v-row justify="space-around" class="ml-12 mb-10">
               <v-col 
                v-for="skill in skills"
                :key="skill.title"
                col="4"
                class="ma-5"
               >
                        <v-list-item-icon>
                            <v-icon class="icon" large> {{ skill.icon}}</v-icon>
                        </v-list-item-icon>

                        <v-list-item-content>
                            <v-list-item-title class="st"> {{ skill.title }}</v-list-item-title>
                        </v-list-item-content>
                       
                    
                </v-col>
        </v-row>
    </v-container>
</template>

<script>
    export default {
        name: "Skills",
        data: () => ({
            skills: [
                { title: 'HTML', icon: 'fab fa-html5'},
                { title: 'CSS', icon: 'fab fa-css3-alt'},
                { title: 'Java Script', icon: 'fab fa-js-square'},
                { title: 'Python', icon: 'fab fa-python'},
                { title: 'VueJS', icon: 'fab fa-vuejs'},
                { title: 'Developing Networks', icon: 'fas fa-hands-helping'},
                { title: 'Problem Solving', icon: 'fas fa-tools'},
                { title: 'Collaborative and Team Oriented', icon: 'fas fa-praying-hands'},
            ]
        })
        
    }
</script>

<style lang="scss" scoped>


</style>