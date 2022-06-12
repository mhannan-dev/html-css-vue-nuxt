<template>
    <div>
        <v-container class="my-12">
            <v-row justify="center">
                <v-col lg="12" class="text-center">
                    <v-subheader class="text-h4 justify-center">Contact</v-subheader>
                    <p class="my-5">
                        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Pariatur
                        blanditiis quod culpa ipsam adipisci. Aliquid quis doloremque
                        assumenda neque hic quos necessitatibus! Recusandae nam facilis
                        nobis vitae, suscipit exercitationem optio.
                    </p>
                </v-col>
                <v-col lg="6">
                    <iframe
                        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d233667.8223908687!2d90.27923710646989!3d23.780887457084543!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3755b8b087026b81%3A0x8fa563bbdd5904c2!2sDhaka!5e0!3m2!1sen!2sbd!4v1654969282549!5m2!1sen!2sbd"
                        width="100%" height="450" style="border:0;" allowfullscreen="" loading="lazy"
                        referrerpolicy="no-referrer-when-downgrade"></iframe>
                </v-col>
                <v-col lg="6">
                    <v-form ref="form">
                        <v-text-field v-model="contactInfo.name" label="Name" :counter="10"
                            required>
                        </v-text-field>
                        <v-text-field v-model="contactInfo.email" label="E-mail" required>
                        </v-text-field>
                        <v-textarea v-model="contactInfo.message" color="teal">
                            <template v-slot:label>
                                <div>
                                    Message
                                </div>
                            </template>
                        </v-textarea>

                        <v-btn color="success" class="mr-4">
                            Submit
                        </v-btn>
                    </v-form>
                </v-col>
            </v-row>
        </v-container>
    </div>
</template>
<script>
export default {
    name: "FooterPart",
    data() {
        return {
            contactInfo: {}
        };
    },
};
</script>

<style lang="css" scoped>
</style>
