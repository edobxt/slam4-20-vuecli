<template>
    <!-- Mon code ici -->
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
</template>

<script>
export default {
    name: "Home",
    data() {
        return {
            // Titre de la barre
            school: "MyDigitalSchool",
            // Élément de la liste
            items: [
                { text: "Premier élément" },
                { text: "Deuxième élément" },
                { text: "Troisième élément" },
            ],
        };
    },
    methods: {
        // Méthode du bouton
        alertOnClick: function() {
            alert("Vous venez de cliquer !");
        },
    },
};
</script>
