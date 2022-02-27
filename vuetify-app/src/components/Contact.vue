<template>
    <v-container>
        <v-row justify="center">
            <v-col lg="12" class="text-center">
                <v-subheader class="text-h4 justify-center">Contact</v-subheader>
                <p>What Services you will Get from me!</p>
            </v-col>
            <v-col lg="6">
                <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3746984.465708819!2d88.10026026270491!3d23.490583053663357!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x30adaaed80e18ba7%3A0xf2d28e0c4e1fc6b!2sBangladesh!5e0!3m2!1sen!2sbd!4v1645185682541!5m2!1sen!2sbd" width="100%" height="100%" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
            </v-col>
            <v-col lg="6">
                <v-form
                    ref="form"

                >
                    <v-text-field
                    v-model="contactInfo.name"
                    :counter="10"
                    label="Name"
                    required
                    ></v-text-field>

                    <v-text-field
                    v-model="contactInfo.email"
                    label="E-mail"
                    required
                    ></v-text-field>
                    <v-textarea label="Messsage" v-model="contactInfo.message">

                    </v-textarea>
                    <v-btn
                    color="success"
                    class="mr-4"
                    >
                    Send
                    </v-btn>
                </v-form>
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
export default {
    name: 'Contact',
    data() {
        return {
            contactInfo:{}
        }
    },
}
</script>

<style scoped>

</style>