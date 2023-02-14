<template>    
    <v-card class="card2 mx-auto" elevation="0">
        <v-card-title style="color:white; max-height: auto;">
           <p class="text-sm-left text-md-center">Estas son mis herramientas amigas.</p>
        </v-card-title>
        <v-card-text id="carText">    
            <v-hover open-delay="200">
                <v-btn v-for="icon in icons" :key="icon" class="mx-10 vBtn" icon>
                    <v-icon :icon="icon.icon" class="i"></v-icon>
                    <v-tooltip bottom :text="icon.text" activator="parent" location="bottom" class="tooltip"></v-tooltip>                    
                </v-btn>
            </v-hover>
        </v-card-text>            
    </v-card>
</template>
<script>
export default {
    name: 'ToolsComponent',
    data() {
        return {
            icons: [
                {'icon':"fas fa-brands fa-php",//php
                "text":"PHP"},
                {"icon":"fas fa-brands fa-laravel",//laravel
                "text":"LARAVEL"},
                {"icon":"fas fa-brands fa-vuejs",//vuejs
                "text":"VUE"},
                {"icon":"fas fa-brands fa-vuejs",//vuetify
                "text":"VUETIFY"},
                {"icon":"fas fa-brands fa-python",//python
                "text":"PYTHON"},
                {"icon":"fas fa-solid fa-database",//mysql
                "text":"MYSQL"},
                {"icon":"fas fa-brands fa-gitlab",//gitlab
                "text":"GITLAB"},
                {"icon":"fas fa-brands fa-github",//github
                "text":"GITHUB"},
                {"icon":"fas fa-brands fa-ubuntu",//linux
                "text":"LINUX"},
                {"icon":"fas fa-sharp fa-solid fa-database",//postgressql
                "text":"POSTGRESSQL"},
                {"icon":"fas fa-brands fa-js",//javascript
                "text":"JAVASCRIPT"},
                {"icon":"fas fa-solid fa-arrows-spin",//apirest
                "text":"APIREST"},
                {"icon":"fas fa-brands fa-jira",//jira
                "text":"JIRA"},
                {"icon":"fas fa-brands fa-docker",//docker
                "text":"DOCKER"}
            ]
        }
    },
}
</script>
<style scoped>
.i{
    font-size: 30px;
    color: orange;
    margin-top: 2%;
    transition: all 0.3s linear;
    text-align: center;
}
.i:hover{
    transform: scale(1.5);
}
.i.text{
    color: green;
}
.card2{
    background-color: #181818;
    max-height: auto;
    display:block;
    font-size: 0;
}
.vBtn{
    background-color: #181818;
    padding: auto;
}
.tooltip{
    transition: all 0.3s linear;
}
.text-center{
    font-family: Mixed;
    font-display: justify;
}
p{
    max-height: auto;
}
#cardText{
    text-align: center;    
}
</style>