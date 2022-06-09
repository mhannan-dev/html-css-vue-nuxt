<template>
    <div>
        <v-container class="my-12">
            <v-row justify="center">
                <v-col lg="12" class="text-center">
                    <v-subheader class="text-h4 justify-center">Projects</v-subheader>
                    <p class="my-5">
                        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Pariatur
                        blanditiis quod culpa ipsam adipisci. Aliquid quis doloremque
                        assumenda neque hic quos necessitatibus! Recusandae nam facilis
                        nobis vitae, suscipit exercitationem optio.
                    </p>
                </v-col>
                <v-col lg="4" v-for="project in 3 " :key="project">
                    <v-card class="mx-auto my-12" max-width="374">
                        <template slot="progress">
                            <v-progress-linear color="deep-purple" height="10" indeterminate></v-progress-linear>
                        </template>
                        <v-img height="250" src="https://cdn.vuetifyjs.com/images/cards/cooking.png"></v-img>
                        <v-card-title>Cafe Badilico</v-card-title>
                        <v-divider class="mx-4"></v-divider>
                        <v-card-actions>
                            <v-btn color="success" rounded>View Details</v-btn>
                            <v-spacer/>
                            <v-rating 
                                color="amber"
                                :value="0.5"
                                dense
                                half-increments
                                readonly
                                size="14"
                            ></v-rating>
                        </v-card-actions>
                    </v-card>
                </v-col>
            </v-row>
        </v-container>
    </div>
</template>
<script>
export default {
    name: "ProjectSection",
    data() {
        return {
            projects: [
                {
                    title: "Web App 1",
                    image:
                        "https://embed-ssl.wistia.com/deliveries/90455478bb71b5642dccd5bbbac98350.jpg",
                },
                {
                    title: "Web App 2",
                    image:
                        "https://cms-assets.tutsplus.com/uploads/users/71/courses/994/preview_image/build-a-restful-api-with-laravel-400x277.png",
                },
                {
                    title: "Web App 2",
                    image:
                        "https://embed-ssl.wistia.com/deliveries/90455478bb71b5642dccd5bbbac98350.jpg",
                },
            ],
        };
    },
};
</script>

<style lang="css" scoped>
</style>
