<template>
  <v-app :style="{ background: $vuetify.theme.themes.dark.background }">
  <NavBar class="ocultar-div"/>
  <v-main>
    <v-container fluid>
      <v-row align="center">
        <div id="home"></div>
        <v-col cols="6">
          <v-img src="perfil.png" contain max-height="200"></v-img>
        </v-col>
        <v-col cols="6" class="justify-text-center">
          <h3 style="color:#B71C1C">¡Hola! Me llamo Héctor</h3>
          <h1 style="color:white">Desarrollador Web</h1>
          <p style="color:grey; text-align: justify; text-justify: inter-word;">
            En crecimiento constante, con experiencia tanto en back-end como en front-end,
            desempeñando labores de creación, mantenimiento, diseño, rediseño y migración de proyectos a nuevas tecnologías
          </p>
        </v-col>
        <v-col cols="12" class="padd">
          <div class="first" id="project">
            <v-row>
              <v-col cols="12">
                <div class="child bgColor1 justify-text-center">
                  <v-icon color="#A7121D" x-large class="ml-3">
                    fa-solid fa-swatchbook
                  </v-icon>
                  <h3 class="ml-3 mt-4" style="color:white">UX Design</h3>
                  <p class="ml-3 mt-6 text-justify" style="color:grey">
                    Enfocando en lo que en verdad <br/> necesita el cliente, su satisfacción y<br/> la mejora continua de la plataforma.
                  </p>
                </div>
                <div class="child bgColor2">
                  <v-icon x-large class="ml-3" dark>fas fa-solid fa-cart-shopping</v-icon>
                  <h3 class="ml-3 mt-4" style="color:white">Product Design</h3>
                  <p class="ml-3 mt-6" style="color:grey" justify>
                    Centrado en la creación de productos<br/> para ayudar a los usuarios a dar sentido<br/> a sus preguntas, a lo complejo y contradictorio<br/> que de vez en cuando llega a la mesa.
                  </p>
                </div>
                <div class="child bgColor1">                
                  <v-icon color="#A7121D" x-large class="ml-3">fas fa-book-open</v-icon>
                  <h3 class="ml-3 mt-4" style="color:white">Metodologías</h3>
                  <p class="ml-3 mt-6 text-center" style="color:grey;">
                    <ul style="list-style:none;">
                      <li>SCRUM</li>
                      <li>AGIL</li>
                      <li>SOLID</li>
                    </ul>
                  </p>
                </div>
              </v-col>
              <v-col cols="12" class="mt-10">
                <div class="child1">
                  <h1 class="text-darken-4 mt-4 number">4</h1>
                  <h3 style="color:white" class="mt-4">Años de experiencia</h3>
                </div>
                <div class="child2 mRight">
                  <v-rom>
                    <v-col cols="12" class="childcol1">
                      <div class="child2 mButton padding bgColor1">
                        <h1 class="text-darken-4 mt-4 number">5</h1>
                        <p style="color:grey">Clientes</p>
                      </div>
                    </v-col>
                    <v-col cols="12" class="childcol1">
                      <div class="child2 padding bgColor1">
                        <h1 class="text-darken-4 mt-4 number">12</h1>
                        <p style="color:grey">Proyectos Completados</p>
                      </div>
                    </v-col>
                  </v-rom>
                </div>
                <div class="child2">
                  <v-rom>
                    <v-col cols="12" class="childcol1">
                      <div class="child2 mButton padding bgColor1">
                        <h1 class="text-darken-4 mt-4 number">2</h1>
                        <p style="color:grey">Compañías</p>
                      </div>
                    </v-col>
                    <v-col cols="12" class="childcol1">
                      <div class="child2 padding bgColor1">
                        <h1 class="text-darken-4 mt-4 number">10</h1>
                        <p style="color:grey">Logros</p>
                      </div>
                    </v-col>
                  </v-rom>
                </div>
              </v-col>
            </v-row>
          </div>
        </v-col>
        <v-col md="3" offset-md="3" id="about">
          <h4 style="color:white">Algunos Proyectos</h4>
          <p style="color:gray">A continuación una muestra de los proyectos que he realizado</p>
        </v-col>
        <v-divider></v-divider>
        <v-col md="3" offset-md="3">
          <v-card height="250px" style="color:#1E1E1E">          
            <v-img src="willis/Willis-motos-1.PNG" cover></v-img>
          </v-card>
          <v-card-actions>
            <v-btn color="#111111" style="color:white" dark text class="ml-n4" append-icon="fas fa-motorcycle">
              Willis motos.
              <v-dialog v-model="modalWillis" activator="parent" width="auto" height="auto">
                <v-card max-width="1000" min-width="auto">
                  <v-card-title>
                    Proyecto realizado con VueJs/Vuetify y Laravel
                  </v-card-title> 
                  <v-card-media>                    
                  <v-carousel show-arrows="hover" delimiter-icon="fas fa-circle" next-icon="fas fa-arrow-right" prev-icon="fas fa-arrow-left">
                    <v-carousel-item>
                      <img src="willis/Willis-motos-1.PNG" style="width: 100%; height: 100%;">
                    </v-carousel-item>
                
                    <v-carousel-item>
                      <img src="willis/Willis-motos-2.PNG" style="width: 100%; height: 100%;">
                    </v-carousel-item>
                
                    <v-carousel-item>
                      <img src="willis/Willis-motos-3.PNG" style="width: 100%; height: 100%;">
                    </v-carousel-item>
  
                    <v-carousel-item>
                      <img src="willis/Willis-motos-4.PNG" style="width: 100%; height: 100%;">
                    </v-carousel-item>
                  </v-carousel>
                  </v-card-media>        
                </v-card>
              </v-dialog>
            </v-btn><br />
          </v-card-actions>
        </v-col>
        <v-col md="3">
          <v-card class="pa-2 py-12" outline tile height="250px" style="color:#1E1E1E">
            <v-img src="claro_collection.PNG" cover></v-img>
          </v-card>
          <v-card-actions>
            <v-btn color="#111111" style="color:white" dark text class="ml-n4" append-icon="fa-sharp fa-solid fa-phone-volume">
              Claro collection.              
              <v-dialog v-model="modalClaro" activator="parent" width="auto" height="auto">
                <v-card max-width="1000" min-width="auto">
                  <v-card-title>
                    Proyecto realizado con VueJs/Vuetify y Laravel
                  </v-card-title> 
                  <v-card-media>                  
                    <v-carousel show-arrows="hover" delimiter-icon="fas fa-circle" next-icon="fas fa-arrow-right" prev-icon="fas fa-arrow-left">
                      <v-carousel-item>
                        <img src="claro_collection.PNG" style="width: 100%; height: 100%;">
                      </v-carousel-item>      
                    </v-carousel>
                  </v-card-media>
                </v-card>
              </v-dialog>
            </v-btn><br />
          </v-card-actions>
        </v-col>
        <v-divider></v-divider>
        <v-col md="3" offset-md="3">
          <v-card class="pa-2 py-12" outline tile height="250px" style="color:#1E1E1E">          
            <v-img cover src="simulador_capacitaciones.PNG" contain style="height: 500px;"></v-img>
          </v-card>
          <v-card-actions>
            <v-btn color="#111111" style="color:white" dark text class="ml-n4" append-icon="fa-solid fa-person-chalkboard">
              Simulador de capacitaciones.
              <v-dialog v-model="modalSimulador" activator="parent" width="auto" height="auto">
                <v-card max-width="1000" min-width="auto">  
                  <v-card-title primary-title>
                    Proyecto realizado con VueJs/Vuetify y Laravel
                  </v-card-title> 
                  <v-card-media>                    
                    <v-carousel show-arrows="hover" delimiter-icon="fas fa-circle" next-icon="fas fa-arrow-right" prev-icon="fas fa-arrow-left">
                      <v-carousel-item>
                        <img src="simulador_capacitaciones.PNG" style="width: 100%; height: 100%;">
                      </v-carousel-item>                
                    </v-carousel>
                  </v-card-media>
                </v-card>
              </v-dialog>
            </v-btn><br />
          </v-card-actions>
        </v-col>
        <v-col md="3">
          <v-card class="pa-2 py-12" outline tile height="250px" style="color:#1E1E1E">
            <v-img cover src="usuarios/usuario-1.PNG" contain style="height: 500px;"></v-img>
          </v-card>
          <v-card-actions>
            <v-btn color="#111111" style="color:white" dark text class="ml-n4" append-icon="fa-solid fa-people-line">
              Usuarios 
              <v-dialog v-model="modalUsuarios" activator="parent" width="auto" height="auto">
                <v-card max-width="1000" min-width="auto">
                  <v-card-title primary-title>
                    Proyecto realizado con VueJs/Vuetify y Laravel
                  </v-card-title>
                  <v-card-media>                    
                    <v-carousel show-arrows="hover" delimiter-icon="fas fa-circle" next-icon="fas fa-arrow-right" prev-icon="fas fa-arrow-left">
                      <v-carousel-item>
                        <img src="usuarios/usuario-1.PNG" style="width: 100%; height: 100%;">
                      </v-carousel-item>
                    
                      <v-carousel-item>
                        <img src="usuarios/usuario-2.PNG" style="width: 100%; height: 100%;">
                      </v-carousel-item>
                    
                      <v-carousel-item>
                        <img src="usuarios/usuario-3.PNG" style="width: 100%; height: 100%;">
                      </v-carousel-item>
      
                      <v-carousel-item>
                        <img src="usuarios/usuario-3.PNG" style="width: 100%; height: 100%;">
                      </v-carousel-item>
                    </v-carousel>
                  </v-card-media>          
                </v-card>
              </v-dialog>
            </v-btn><br />
          </v-card-actions>
        </v-col>
        <v-col cols="auto" align-self="center" justify="space-between">
          <ToolsComponent />
        </v-col>
        <v-col cols="12" class="padd topInverse">
          <div class="second">
            <div class="secondchild1" id="contact">
              <v-row>
                <v-col cols="7">
                  <h3 style="color:white">
                    ¡Gracias por tu visita!<br />
                  </h3>
                  <p style="color:grey">
                    Si quieres contactarme y saber más sobre mi trabajo,
                          da click. <br />
                  </p>
                </v-col>
                <v-col cols="5">
                  <v-btn tile color="#A7121D" dark class="mt-16" >
                    <a href="mailto:postulantehuertas@gmail.com" style="color:white">Contact</a>
                    </v-btn>
                </v-col>
              </v-row>            
            </div>
          </div>
          <v-toolbar class="topTolbar" color="#111111" dark flat>
            <div style="position: absolute; margin-left: auto; margin-right:auto; left: 0; right: 0; text-align: center">
              <v-btn color="white" text @click="scroll('app')">Inicio</v-btn>
              <v-btn color="white" text @click="scroll('project')">Experiencia</v-btn>
              <v-btn color="white" text @click="scroll('about')">Proyectos</v-btn>
              <v-btn color="white" text @click="scroll('contact')">Contacto</v-btn>
            </div>
          </v-toolbar>
        </v-col>
      </v-row>
    </v-container>
    <FooterComponent />
  </v-main>
  </v-app>
  </template>
  
  <script>
  import NavBar from './components/NavBar.vue'
  import FooterComponent from './components/FooterComponent.vue'
  import ToolsComponent from './components/ToolsComponent.vue';
  
  export default {
    name: 'App',
  
    components: {
      NavBar,
      FooterComponent,
      ToolsComponent
    },
    data() {
      return {
        items: [
          {
            value: 'SCRUM',
          },
          {
            value: 'AGIL',
          },
          {
            value: 'SOLID',
          },
        ],
        modalWillis:false,
        modalUsuarios:false,
        modalClaro:false,
        modalSimulador:false
      }
    },
    methods: {
      scroll(refName) {
        const element = document.getElementById(refName);
        element.scrollIntoView({ behavior: "smooth" });
      },
      openModalWillis(){
        this.modalWillis = true;
      },
      openModalUsuarios(){
        this.modalUsuarios = true;
      },
      openModalClaro(){
        this.modalClaro = true;
      },
      openModalSimulador(){
        this.modalSimulador = true;
      }
    },
  }
  </script>
  <style scoped>
  .topInverse{
    margin-top: -250px;
  }
  .topTolbar {
    margin-top: 100px;
    text-align: center;
  }
  
  .first {
    width: 100%;
    height: 100%;
    background: linear-gradient(
      to right,
      #181818,
      #181818 50%,
      #111111 50%,
      #111111 50%
    );
    text-align: center;
    padding: 2rem 2rem;
  }
  
  .second {
    width: 100%;
    height: 400px;
    background: #181818;
    text-align: center;
    padding: 2rem 2rem;
  }
  
  .secondchild1 {
    display: inline-block;
    background-color: #1e1e1e;
    padding: 2rem 1rem;
    vertical-align: middle;
    text-align: left;
    margin-top: 250px;
  }
  
  .child{
    display: inline-block;
    padding: 2rem 1rem;
    vertical-align: middle;
    text-align: left;
    margin-right: 8px;
  }
  
  .bgColor1{
    background-color: #1e1e1e;
  }
  
  .bgColor2{
    background-color: #ce1d2a;
  }
  .child1{
    display: inline-block;
    padding: 2rem 1rem;
    vertical-align: middle;
    margin-right: 5px;
    width: 240px;
  }
  
  .child2 {
    display: inline-block;
    width: 245px;
    vertical-align: middle;
  }
  
  .mRight{
    margin-right: 8px;
  }
  
  .mButton{
    margin-bottom: 8px;
  }
  
  .padding {
    padding: 8px 0px;
  }
  
  .col-12.padd{
    padding: 12px 0 !important;
  }
  
  .col-12.childcol {
    padding: 0 !important;
  }
  
  h1.number {
    font-size: 50px;
    font-weight: bold;
    color:#A7121D !important;
    opacity:0.6
  }
  
  h5{
    font-family: fantasy;
  
  }

  @media screen and (max-width: 600px){
    .ocultar-div{
      display: none;
    }
  }
  </style>