<template>
    <v-footer class="blackFooter">
      <v-card
        class="card"
      >
        <v-row>
          <v-col cols="12" sm="4">
            <v-card-text class="white--text pt-2">
              <v-btn icon id="vBtn">
                <v-icon>fa-brands fa-connectdevelop</v-icon>
              </v-btn>
            </v-card-text>
          </v-col>
  
          <v-col cols="12" sm="4">
            <v-card-text class="pt-2">
              <v-btn
                v-for="icon in icons"
                :key="icon"
                class="mx-1"
                icon
                id="vBtn"
              >
              <a target="_blank" class="fcc-btn" :href="icon.url">
                <v-icon>
                    {{ icon.icon }}
                </v-icon>
              </a>
              </v-btn>
            </v-card-text>
          </v-col>
          <v-col cols="12" sm="4">
            <v-card-text class="pt-2">
              <v-btn class="mx-1" icon id="vBtn">
                <v-icon>fas fa-heart</v-icon>
              </v-btn>
              Created with love
            </v-card-text>
          </v-col>
        </v-row>
      </v-card>
    </v-footer>
  </template>
<script>
export default {
    name: 'FooterComponent',
    data() {
        return {
            icons: [
                {"icon":"fas fa-brands fa-google","url":"mailto:postulantehuertas@gmail.com"},
                {"icon":"fas fa-brands fa-linkedin","url":"https://www.linkedin.com/in/hector-huertas-062466287/"},
                {"icon":"fas fa-brands fa-gitlab","url":"https://gitlab.com/hyhuertas"}
            ]
        }
    },
}
</script>

<style>
.blackFooter{
  background-color: #181818;
  padding: 0,0 !important;
  margin-left: auto;
  margin-right: auto;
}

.card{
  background-color: black;
  color:white;
  width: 100%;
  text-align: center;
}

#vBtn{
  background:black;
  color:red
}

a{
  color: red;
}
</style>
