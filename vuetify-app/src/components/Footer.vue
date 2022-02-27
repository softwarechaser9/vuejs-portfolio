<template>
    <v-footer padless>
        <v-col lg="12">
            <v-row justify="center">
                <v-col lg="4" class="text-center">
                    <v-toolbar-title>software hunt</v-toolbar-title>
                    <v-card-text>
                <v-btn
                v-for="icon in icons"
                :key="icon"
                class="mx-4 white--black"
                icon
                >
                <v-icon size="24px">
                    {{ icon }}
                </v-icon>
                </v-btn>
            </v-card-text>
            <v-subheader>Naything</v-subheader>
            <v-form>
                <v-text-field label="Email" outlined dense />
                    <v-btn rounded color="success">Subscribe Us</v-btn>
            </v-form>
                </v-col>
                
            </v-row>
            <div class="mt-10">
                    <v-divider></v-divider>
                    <v-subheader>
                        @ Copyright software hunt. All Rights Reserved {{ new Date().getFullYear() }} — <strong>Vuetify</strong> <v-spacer></v-spacer>
                        <strong> Md. Shohanur Rahman</strong>
                    </v-subheader>
                </div>
        </v-col>
        </v-footer>
</template>

<script>
export default {
    name: "Footer",
    data() {
        return {
            icons: [
        'mdi-facebook',
        'mdi-twitter',
        'mdi-linkedin',
        'mdi-instagram',
        ],
        }
    },
}
</script>


<style scoped>

</style>