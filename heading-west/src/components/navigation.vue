<template>
    <span>
        <v-navigation-drawer app v-model="drawer" class="black" dark disable-resize-watcher>
            <v-list>
                <template v-for="(item, index) in items">
                    <v-list-tile :key="index">
                        <v-list-tile-content>
                            {{item.title}}
                        </v-list-tile-content>
                    </v-list-tile>
                    <v-divider :key="`divider-${index}`"></v-divider>
                </template>
            </v-list>
        </v-navigation-drawer>
        <v-toolbar app color="black" >
            <v-toolbar-side-icon class="hidden-md-and-up" @click="drawer = !drawer"></v-toolbar-side-icon>
            <v-spacer class="hidden-md-and-up"></v-spacer>
            <router-link to="/">
                <v-toolbar-title to="/">{{appTitle}}</v-toolbar-title>
            </router-link>
            <v-btn flat class="hidden-sm-and-down" to="/hello">About H&D</v-btn>
            <v-spacer class="hidden-sm-and-down"></v-spacer>
            <v-btn flat class="hidden-sm-and-down" to="/bookus">Book Us!</v-btn>
        </v-toolbar>
    </span>
</template>
<script>

export default {
    name: 'navigation',
    data() {
        return {
            appTitle: 'Headin\' West',
            drawer: false,
            items: [
                { title: 'About H&D' },
                { title: 'Book Us' },
            ]
        };
    }
};
</script>
<style scoped>
a {
    color: white;
    text-decoration: none;
}
</style>