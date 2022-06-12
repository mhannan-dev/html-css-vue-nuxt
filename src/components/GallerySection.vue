<template>
    <div>
        <v-container class="my-12">
            <v-row justify="center">
                <v-col lg="12" class="text-center">
                    <v-subheader class="text-h4 justify-center">Gallery</v-subheader>
                    <p class="my-5">
                        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Pariatur
                        blanditiis quod culpa ipsam adipisci. Aliquid quis doloremque
                        assumenda neque hic quos necessitatibus! Recusandae nam facilis
                        nobis vitae, suscipit exercitationem optio.
                    </p>
                </v-col>
                <v-col cols="3" v-for="gallery in 9" :key="gallery" class="d-flex child-flex">
                    <v-img cols="6" sm="4" lazy-src="https://picsum.photos/id/11/10/6" max-height="150" max-width="250"
                        src="https://picsum.photos/id/11/500/300"></v-img>
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
