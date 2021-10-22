<template>
  <div id="app">
    <div id="nav">
      <img src="./assets/agenda.svg" alt="icone d'accès à l'agenda">
      <img src="./assets/image.svg" alt="icone d'accès à la galerie d'image">
      <router-link to="/"><img src="./assets/home.svg" alt="icone d'accès à l'accueil"></router-link>


      <img src="./assets/contact.svg" alt="icone d'accès au formulaire de contact">
      <router-link to="/about"><img src="./assets/information.svg" alt="icone d'accès à la partie à propos"></router-link>
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
  padding: 30px;
  position: fixed;
  bottom: 0px;
  display: flex;
  width: 100%;
  justify-content: space-around;
  align-items: center;
  background-color: white;
  border-top: 1px gray solid;
  margin: 0%;
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
</style>
