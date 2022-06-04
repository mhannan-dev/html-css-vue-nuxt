<template>
    <div>
        <v-container class="my-12">
            <v-row justify="center">
                <v-col lg="12" class="text-center">
                    <v-subheader class="text-h4 justify-center">My Portfolio</v-subheader>
                    <p class="my-5">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Pariatur blanditiis quod
                        culpa ipsam adipisci. Aliquid quis doloremque assumenda neque hic quos necessitatibus!
                        Recusandae nam facilis nobis vitae, suscipit exercitationem optio.</p>
                </v-col>
                <v-col lg="12" class="text-center">
                    <div class="text-center">
                        <v-chip @click="activePortfolio = 'web'" :color="activePortfolio == 'web' ? 'success' : ''"
                            class="mx-5">Laravel</v-chip>
                        <v-chip @click="activePortfolio = 'frontend'"
                            :color="activePortfolio == 'frontend' ? 'success' : ''" class="mx-5">Front End</v-chip>
                        <v-chip @click="activePortfolio = 'wordpress'"
                            :color="activePortfolio == 'wordpress' ? 'success' : ''" class="mx-5">Wordpress</v-chip>
                    </div>
                </v-col>
                <slot v-if="activePortfolio == 'web'">
                    <v-col lg="3" v-for="(web, webIndex) in webApps" :key="webIndex">
                        <v-card>
                            <v-img class="white--text align-end" gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                                height="200" :src="web.image">
                                <v-card-title>{{ web.title }}</v-card-title>
                            </v-img>
                        </v-card>
                    </v-col>
                </slot>
                <slot v-if="activePortfolio == 'frontend'">
                    <v-col lg="3" v-for="(front, frontIndex) in frontend" :key="frontIndex">
                        <v-card>
                            <v-img class="white--text align-end" gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                                height="200" :src="front.image">
                                <v-card-title>{{ front.title }}</v-card-title>
                            </v-img>
                        </v-card>
                    </v-col>
                </slot>
                <slot v-if="activePortfolio == 'wordpress'">
                    <v-col lg="3" v-for="(wp, wpIndex) in wordpress" :key="wpIndex">
                        <v-card>
                            <v-img class="white--text align-end" gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                                height="200" :src="wp.image">
                                <v-card-title>{{ wp.title }}</v-card-title>
                            </v-img>
                        </v-card>
                    </v-col>
                </slot>
            </v-row>
        </v-container>
    </div>
</template>
<script>
export default {
    name: 'PortfolioSection',
    data() {
        return {
            activePortfolio: 'web',
            webApps: [
                { title: 'Web App 1', image: 'https://embed-ssl.wistia.com/deliveries/90455478bb71b5642dccd5bbbac98350.jpg' },
                { title: 'Web App 2', image: 'https://cms-assets.tutsplus.com/uploads/users/71/courses/994/preview_image/build-a-restful-api-with-laravel-400x277.png' },
                { title: 'Web App 2', image: 'https://embed-ssl.wistia.com/deliveries/90455478bb71b5642dccd5bbbac98350.jpg' },
                { title: 'Web App 4', image: 'https://cdn.slidesharecdn.com/ss_thumbnails/solid-150219094748-conversion-gate01-thumbnail-4.jpg?cb=1424350800' }
            ],
            frontend: [
                { title: 'Frontend App 1', image: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/vue-black-dashboard-pro/vue-black-dashboard-pro.jpg' },
                { title: 'Frontend App 2', image: 'https://cdn.vuetifyjs.com/images/cards/cooking.png' },
                { title: 'Frontend App 2', image: 'https://miro.medium.com/max/1400/1*mh8il3s3hB0Xdpx6ffQLTw.png' },
                { title: 'Frontend App 4', image: 'https://cdn.vuetifyjs.com/images/cards/cooking.png' }
            ],
            wordpress: [
                { title: 'Wordpress App 1', image: 'https://149611589.v2.pressablecdn.com/wp-content/uploads/2018/10/Screen-Shot-2018-10-30-at-7.59.17-PM.png' },
                { title: 'Wordpress App 2', image: 'https://www.e2msolutions.com/wp-content/uploads/2021/08/banner-woocommerce-img.png' },
                { title: 'Wordpress App 2', image: 'https://5.imimg.com/data5/OG/WP/MY-18188724/wordpress-theme-development-500x500.jpg' },
                { title: 'Wordpress App 4', image: 'https://www.wpcreative.com.au/wp-content/uploads/2016/04/wp-plugins-deve.jpg' }
            ]
        }
    }
}
</script>

<style lang="css" scoped>
</style>