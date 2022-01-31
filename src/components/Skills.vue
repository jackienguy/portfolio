<template>
    <v-container>
        <v-row>
            <v-col cols="4" md="8" class="ml-12 mt-12 mb-12">
                <h1>Skills and Competencies</h1>
            </v-col>
        </v-row>

        <v-row justify="space-around" class=" mb-10">
               <v-col class="d-flex justify-start">
                
                    <v-list-item
                        v-for="skill in skills"
                        :key="skill.title"
                    >
                        <v-list-item-icon>
                            <v-icon large color="blue darken-2"> {{ skill.icon}}</v-icon>
                        </v-list-item-icon>

                        <v-list-item-content>
                            <v-list-item-title> {{ skill.title }}</v-list-item-title>
                        </v-list-item-content>
                        </v-list-item>
                    
                </v-col>
                





                    <!-- <v-icon large color="blue darken-2"> fab fa-html5 </v-icon>
                    HTML
                </v-col>

                 <v-col class="d-flex" cols="6" md="2">
                    <v-icon large color="purple darken-2"> fab fa-css3-alt </v-icon>
                    CSS
                </v-col>

                 <v-col class="d-flex" cols="6" md="2">
                    <v-icon large color="green darken-2"> fab fa-js-square</v-icon>
                    Java Script
                </v-col>

                 <v-col class="d-flex" cols="6" md="2">
                    <v-icon large color="blue darken-2"> fab fa-python</v-icon>
                    Python
                </v-col>

                 <v-col class="d-flex" cols="6" md="3">
                    <v-icon large color="green darken-2">fab fa-vuejs</v-icon>
                    VueJS
                </v-col>
        </v-row>

        <v-row justify="space-around" class="flex-child mb-12">
            <v-col class="d-flex" cols="6" md="3">
                <v-icon large color="green darken-2">fas fa-hands-helping</v-icon>
                Developing Networks
            </v-col>

            <v-col class="d-flex" cols="6" md="3">
                <v-icon large color="green darken-2">fas fa-praying-hands</v-icon>
                Collaborative and Team Oriented
            </v-col>

            <v-col class="d-flex" cols="6" md="3">
                <v-icon large color="green darken-2">fas fa-tools</v-icon>
                Problem Solving -->
            
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