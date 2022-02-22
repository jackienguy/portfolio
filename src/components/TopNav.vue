<template>
    <v-container width="100vw">
        <div class="d-flex justify-end mb-2">
            <!-- Mobile Menu Icon -->
             <v-btn id="toggleBtn"
            @click="overlay = !overlay"
            class="mx-2 pa-9"
            fab
            >
                <v-icon dark dense color="black" >
                    fas fa-bars
                </v-icon>
            </v-btn>

            <v-btn class="navBtn ml-5"
            v-for="link in links"
            :key="link"
            text
            >
                {{ link }}
            </v-btn>
        </div>
        <div>
<!--           
            <v-navigation-drawer 
                v-model="navDrawer"
                temporary
                absolute
                width="50vw"
                >
                <v-list class="mt-12 pt-12" dense>
                    <v-list-item 
                    v-for="(link) in links"
                    :key="link"
                    text
                    >
                        {{ link }}
                    </v-list-item>
                </v-list>
               
              
            
            </v-navigation-drawer> -->
            <div id="overlay-menu">
                 <v-overlay 
            
                :absolute="absolute"
                :value="overlay"
                height="100vh"
                width="100vw"
                >
                <v-btn id="closeOverlayBtn"
                @click="overlay = false"
                class="mx-2 pa-9"
                fab
                >
                close
                </v-btn>

                 <v-list class="mt-12 pt-12" dense>
                    <v-list-item 
                    v-for="(link) in links"
                    :key="link"
                    text
                    >
                        {{ link }}
                    </v-list-item>
                </v-list>

            </v-overlay>
            </div>
           
           
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
            navDrawer: null,
            absolute: true,
            overlay: false
        })
    }
</script>

<style lang="scss" scoped>
    // for small screen 
    
    #toggleBtn {
        cursor: pointer;
    }

    #overlay-menu {
        transition: 0.5s;
        z-index: 1;
        overflow: hidden;
    }


    // for medium screen 
    @media screen and (min-width: 880px) {
        #toggleBtn {
            display: none;
        }
    }

    @media screen and (max-width: 880px) {
        .navBtn {
            display: none;
        }
    }

</style>