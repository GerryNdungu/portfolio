<template>
    <v-footer dark padless>
        <v-card tile flat class="black white--text py-5 px-5 text-center" width="100%">
            <v-row>
                <v-col cols="12" sm="4">
                    <v-card-text class="white--text pt-2">
                        <v-btn icon>
                            <v-icon color="#A7121D">fas fa-dragon</v-icon>
                        </v-btn>
                    </v-card-text>
                </v-col>
                <v-col cols="12" sm="4">
                    <v-card-text class="pt-2">
                        <v-btn v-for="icon in icons" :key="icon" class="mx-1 white--text" icon>
                            <v-icon size="24px">
                                {{ icon }}    
                            </v-icon>
                        </v-btn>
                    </v-card-text>
                </v-col>
                <v-col cols="12" sm="4">
                    <v-card-text class="pt-2">
                        <v-btn class="mx-1 white--text" icon>
                            <v-icon color="#A7121D">fa-heart </v-icon>
                        </v-btn>    
                        Created by Gerry J
                    </v-card-text>
                </v-col>
            </v-row>
        </v-card>
    </v-footer>
</template>

<script>
export default {
    name:"FooterBar",
    data:()=>({
        icons:["mdi-facebook","mdi-twitter","mdi-linkedin","mdi-instagram","mdi-github"]
    }),
    setup () {
        

        return {}
    }
}
</script>

<style lang="scss" scoped>

</style>