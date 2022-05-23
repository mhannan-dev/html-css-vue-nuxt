<template>
    <div>
        <v-app-bar app color="white" elevation="6" elevate-on-scroll style="padding: 0px 90px">
            <v-toolbar-title> Hello World </v-toolbar-title>
            <v-spacer />
            <v-list class="d-flex align-center">
                <v-list-item v-for="(menu, index) in menus" :key="index">
                    <v-list-item-title> {{ menu.title }} </v-list-item-title>
                </v-list-item>
                <v-btn text>
                    <v-icon>mdi-magnify</v-icon>
                </v-btn>
                <v-btn outlined color="success"> Get Started </v-btn>
            </v-list>
        </v-app-bar>
    </div>
</template>
<script>
export default {
    name: "AppHeader",
    data() {
        return {
            menus: [
                { title: 'Home', route: 'home' },
                { title: 'About us', route: 'about-us' },
                { title: 'Portfolio', route: 'portfolio' },
                { title: 'Projects', route: 'projects' },
                { title: 'Gallery', route: 'gallery' },
                { title: 'Contact', route: 'contact' },
            ],
        }
    }
};
</script>
<style lang="scss" scoped>
</style>
