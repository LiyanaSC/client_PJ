<template>
  <div id="app">
    <div id="nav">
      <router-link to="/agenda"><img class="" src="./assets/agenda.svg" alt="icone d'accès à l'agenda"></router-link >
      <router-link to="/gallery"><img class="" src="./assets/image.svg" alt="icone d'accès à la galerie d'image"></router-link >
      <router-link to="/"><img class="" src="./assets/home.svg" alt="icone d'accès à l'accueil"></router-link>


      <router-link to="/contact"><img class="" src="./assets/contact.svg" alt="icone d'accès au formulaire de contact"></router-link >
      <router-link to="/about"><img class="info" src="./assets/information.svg" alt="icone d'accès à la partie à propos"></router-link>
    </div>
    <router-view/>
  </div>
</template>

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
  width: 100%;
  justify-content: space-around;
  align-items: center;
  background-color: white;
  border-top: 1px gray solid;
  margin: 0%;
  height: 100px;
  max-height: 100px;
  z-index: 10;

 
  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
  img{
    max-height: 50px;
  }
  
}
.info{
  margin: 0px;
  padding: 4px;
  border: 2px black solid;
  border-radius: 50%;
  height: 40px;
}
</style>
