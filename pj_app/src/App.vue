<template>
  <div id="app">

    <div id="nav">
      <router-link to="/" @click.native="scrollToTop"><img class="icon_menu home" src="./assets/home.svg" alt="icone d'accès à l'accueil"><p class="text_menu">Accueil </p></router-link>

      <router-link to="/agenda" @click.native="scrollToTop"><img class="icon_menu" src="./assets/agenda.svg" alt="icone d'accès à l'agenda"><p class="text_menu">Agenda </p></router-link >
      <router-link to="/gallery" @click.native="scrollToTop"><img class="icon_menu" src="./assets/image.svg" alt="icone d'accès à la galerie d'image"><p class="text_menu">Galerie </p></router-link >


      <router-link to="/contact" @click.native="scrollToTop"><img class="icon_menu" src="./assets/contact.svg" alt="icone d'accès au formulaire de contact"><p class="text_menu">Réserver </p></router-link >
      <router-link to="/about" @click.native="scrollToTop"><img class="icon_menu info" src="./assets/information.svg" alt="icone d'accès à la partie à propos"><p class="text_menu">À propos</p></router-link>
    </div>
     <Headerlogo/>

    <router-view/>
  </div>
</template>

<script>
import Headerlogo from './components/Headerlogo.vue'
export default {
  components: { Headerlogo },
  setup() {
    
  },
  methods:{
     scrollToTop() {
                window.scrollTo(0,0);
           }
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: 0%;
}

#nav {
  
  position: fixed;
  bottom: 0px;
  display: flex;
  flex-direction: row;
  width: 100%;
  justify-content: space-around;
  align-items: center;
  background-color: white;
  border-top: 1px gray solid;
  margin: 0%;
  height: 100px;
  max-height: 100px;
  z-index: 10;
  @media screen and (min-width: 900px) {
    position: relative;
    border: none;
    justify-content: right;
    
  }
 
  a {
     text-decoration: none;
    font-weight: bold;
    color: #2c3e50;
    @media screen and (min-width: 900px) {
        position: relative;
        border: none;
        justify-content: right;
         &.router-link-exact-active {
            color: palevioletred;
            border-bottom: 2px palevioletred solid;
          }
        &:hover{
                     color: palevioletred;
 
        }
      }
   
  }
  img{
    max-height: 50px;
  }
  
}
.icon_menu{
  @media screen and (min-width: 900px) {
    display: none;
  }
}
#nav :nth-child(1) { 
  @media screen and (max-width: 899px) {
  order: 3; 
  }
  }
#nav :nth-child(2) { 
  @media screen and (max-width: 899px) {
  order: 1; 
  }
  }  
#nav :nth-child(3) { 
  @media screen and (max-width: 899px) {
  order: 2; 
  }
  }
#nav :nth-child(4) { 
  @media screen and (max-width: 899px) {
  order: 4; 
  }
  }
#nav :nth-child(5) { 
  @media screen and (max-width: 899px) {
  order: 5; 
  }
  }

.text_menu{
  display: none;
@media screen and (min-width: 900px) {
    display: initial;
    font-size: 1.5rem;
    margin-right: 10px;
    margin-left: 10px;
   
  }
}
.info{
  margin: 0px;
  padding: 4px;
  border: 2px black solid;
  border-radius: 50%;
  height: 40px;
}
.btn_style{
  border: none;
  border-radius: 25px 25px 25px 25px ;
  height: 50px;
  background-color: palevioletred;
  color: #fff;
  font-weight: bold;
  padding-left:15px;
  padding-right: 15px;
      box-shadow: 1px 1px 2px grey;

  &:hover{
    box-shadow: 1px 1px 5px rgb(0, 0, 0);
  }
  &:active{
    box-shadow: 2px 2px 5px rgb(0, 0, 0);
  }

}
.btn_color_two{
background-color:rgb(91, 182, 218) ;
}
.customer{
    @media screen and (min-width: 900px) {
      order:7;
      width: 90%;
  
    }

}
</style>
