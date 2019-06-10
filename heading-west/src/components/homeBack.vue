<template>
    <v-container fluid fill-height class="home-back" style="max-height: 100vh;">>
        <v-layout justify-center align-center column pa-5>
            <div class="display-4 font-weight-black white--text text-xs-center">COUNTRY MUSIC</div>
            <div class="display-4 font-weight-black white--text text-xs-center mb-3">FOR YOUR EVENTS</div>
            <div class="display-1 font-weight-bold white--text text-xs-center">Give your events the down home feeling of yesteryear.</div>
            <v-btn fab class="mt-5 brown darken-4">
            <v-icon large color="white">expand_more</v-icon>
            </v-btn>
        </v-layout>
    </v-container>
</template>

<script>
export default {
    name: 'homeBack'
};
</script>

<style scoped>
.home-back {
    background: url('http://source.unsplash.com/URlcLAfyYGU');
    background-size: cover;
    width: 100%;
    height: 100%;
}
</style>