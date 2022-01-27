<template>
    <v-container width="100vw">
        <div class="d-flex justify-end mb-2">
            <!-- Mobile Menu Icon -->
             <v-btn id="toggleBtn"
            @click="navDrawer = !navDrawer"
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
               
              
            
            </v-navigation-drawer>
           
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
            navDrawer: null
        })
    }
</script>

<style lang="scss" scoped>
    // for small screen 
    
    #toggleBtn {
            cursor: pointer;
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