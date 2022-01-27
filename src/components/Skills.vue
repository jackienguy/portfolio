<template>
    <v-container>
        <v-row>
            <v-col cols="4" class="ml-12 mt-12 mb-12">
                <h1>Skills</h1>
            </v-col>
        </v-row>

        <v-row justify="space-around" class="flex-child mb-10">
                <v-col class="d-flex" cols="6" md="2">
                    <v-icon large color="blue darken-2"> fab fa-html5 </v-icon>
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
                Problem Solving
            </v-col>
        </v-row>
        
    </v-container>
    

</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>

</style>