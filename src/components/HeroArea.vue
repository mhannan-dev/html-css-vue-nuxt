<template>
    <div>
        <v-container>
            <v-row>
                <v-col lg="6">
                    <h1 class="hero-heading">Welcome to our VueJS/Vuetify App</h1>
                    <p class="hero-description">Lorem ipsum dolor sit amet consectetur adipisicing elit. Minima vel
                        placeat optio incidunt, quo dignissimos illum fugiat enim unde delectus nesciunt architecto
                        consectetur adipisci dolorum numquam! Repellendus quibusdam itaque a.</p>
                    <v-btn class="white-text mr-4" color="success" rounded>Get Started</v-btn>
                    <v-btn class="white-text" color="indigo" rounded>
                        <v-icon>mdi-play-circle</v-icon>Watch
                    </v-btn>
                </v-col>
                <v-col lg="6">
                    <img src="../assets/693.png" alt="Image" width="100%">
                </v-col>
            </v-row>
        </v-container>
    </div>
</template>

<script>
export default {
    name: 'HeroArea',
}
</script>

<style lang="css" scoped>
.hero-heading{
    font-size: 50px;
    font-weight: bold;
    letter-spacing: 2.5px;
    font-family: revert;
}
.hero-description{
    margin: 1.5rem 0rem;
    font-size: inherit;
    letter-spacing: 0.9px;
    line-height: inherit;
}
</style>