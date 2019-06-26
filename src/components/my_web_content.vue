<template>
    <div>
        <v-layout>
            <v-flex xs12 sm6 offset-sm3>
                <v-card>
                    <v-img src="./../assets/card_img.jpg" aspect-ratio="2.75"></v-img>
                    <v-card-title primary-title>
                        <div>
                            <h3 class="headline mb-0">Kangaroo Valley Safari</h3>
                            <div> {{ card_text }} </div>
                        </div>
                    </v-card-title>
                    <v-card-actions>
                        <v-btn depressed color="orange">ddShare</v-btn>
                        <v-btn flat color="orange">Explore</v-btn>
                    </v-card-actions>
                </v-card>
            </v-flex>
        </v-layout>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                card_text : 'dfdfdfdfd'
            }
        },
        components: {

        }
    }
</script>

<style>
    p {
        position: relative;
        z-index: 0;
    }
</style>