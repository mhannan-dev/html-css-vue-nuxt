<template>
    <div>
        <v-container>
            <v-row>
                <v-col lg="4">
                    <img src="../assets/8401.png" alt="Image" width="100%">
                </v-col>
                <v-col lg="8">
                    <h4 class="about-heading">I am Muhammad Hannan</h4>
                    <p class="about-description">Lorem ipsum dolor sit amet consectetur adipisicing elit. Minima vel
                        placeat optio incidunt, quo dignissimos illum fugiat enim unde delectus nesciunt architecto
                        consectetur adipisci dolorum numquam! Repellendus quibusdam itaque a.</p>
                    <v-list-item>
                        <v-icon color="success" class="mr-2">mdi-check-all &nbsp;</v-icon>
                        <v-list-item-subtitle>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Suscipit quasi ut autem soluta placeat odio ad pariatur laborum veritatis, asperiores perferendis obcaecati nesciunt quaerat tempore molestiae voluptatum! Totam, deserunt error!</v-list-item-subtitle>
                    </v-list-item>    
                    <v-list-item>
                        <v-icon color="success" class="mr-2">mdi-check-all &nbsp;</v-icon>
                        <v-list-item-subtitle>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Suscipit quasi ut autem soluta placeat odio ad pariatur laborum veritatis, asperiores perferendis obcaecati nesciunt quaerat tempore molestiae voluptatum! Totam, deserunt error!</v-list-item-subtitle>
                    </v-list-item>    
                    <v-btn class="white-text mt-4" color="success" rounded>Get Started</v-btn>
                </v-col>
            </v-row>
        </v-container>
    </div>
</template>

<script>
export default {
    name: 'AboutUs',
}
</script>

<style lang="css" scoped>
.about-heading {
    font-size: 35px;
    font-weight: bold;
    letter-spacing: 2.5px;
    font-family: revert;
}

.about-description {
    margin: 1.5rem 0rem;
    font-size: inherit;
    letter-spacing: 0.9px;
    line-height: inherit;
}
</style>