<template>
    <v-app>
        <v-app-bar app color="primary" dark>
            <v-toolbar-title>{{ school }}</v-toolbar-title>
        </v-app-bar>

        <v-main>
            <div class="text-center pa-10">👋🏾 Bonjour 👋🏾</div>
            <!-- Mon code -->
            <!-- Ajout du bouton -->
            <v-btn block v-on:click="alertOnClick">Clique ici</v-btn>
            <br />
            <!-- Ajout de la card -->
            <v-card color="#385F73" dark>
                <v-card-text>Ceci est une card</v-card-text>
            </v-card>
            <br />
            <!-- Ajout de la liste -->
            <v-list-item>
                <v-list-item-content v-for="(item, i) in items" :key="i">
                    <v-list-item-title> {{ item.text }} </v-list-item-title>
                </v-list-item-content>
            </v-list-item>
        </v-main>
    </v-app>
</template>

<script>
export default {
    name: "App",
    data() {
        return {
            school: "MyDigitalSchool",
            items: [
                { text: "Premier élément" },
                { text: "Deuxième élément" },
                { text: "Troisième élément" },
            ],
        };
    },
    methods: {
        alertOnClick: function() {
            alert("Vous venez de cliquer !");
        },
    },
};
</script>
