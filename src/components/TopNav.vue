<template>
    <v-container>
        <div class="d-flex justify-space-around mb-4">
            <!-- Mobile Menu Icon -->
             <v-btn id="toggleBtn"
            class="mx-2 pa-9"
            fab
            color="teal"
            >
                <v-icon dark dense color="yellow" >
                    I
                </v-icon>
            </v-btn>

            <v-btn id="navBtn"
            v-for="link in links"
            :key="link"
            text
            >
                {{ link }}
            </v-btn>
        </div>
    </v-container>
</template>

<script>
    export default {
        name: "TopNav",
        data: () => ({
            links: [
                'Skills',
                'Projects',
                'Resume',
                'Contact',
            ],
        })
    }
</script>

<style lang="scss" scoped>
    // for small screen 
    
    #toggleBtn {
            margin: 60px 10px 20px;
            cursor: pointer;
        }

    // for medium screen 
    @media screen and (min-width: 990px) {
        #toggleBtn {
            display: none;
        }
    }

</style>