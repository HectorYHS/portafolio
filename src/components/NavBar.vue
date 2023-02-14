<template>
    <v-app-bar app color="#111111" dark flex class="px-8" id="home">
        <v-btn icon color="#A7121D">
            <v-icon icon="fa-brands fa-connectdevelop" />
        </v-btn>
        <v-spacer></v-spacer>
        <v-btn color="white" text @click="scroll('app')">Inicio</v-btn>
        <v-btn color="white" text @click="scroll('project')">Experiencia</v-btn>
        <v-btn color="white" text @click="scroll('about')">Proyectos</v-btn>
        <v-btn color="white" text @click="scroll('contact')">Contacto</v-btn>
    </v-app-bar>
</template>
<script>
export default {
    methods: {
        scroll(refName) {
            const element = document.getElementById(refName);
            element.scrollIntoView({behavior: "smooth"});
        }
    },

}
</script>
<style>
</style>