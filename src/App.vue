<template>
    <v-app>
        <v-app-bar app color="primary" dark>
            <v-toolbar-title>{{ school }}</v-toolbar-title>
        </v-app-bar>

        <Home />
    </v-app>
</template>

<script>
import Home from "./components/Home.vue";
export default {
    name: "App",
    components: {
        Home,
    },
};
</script>
