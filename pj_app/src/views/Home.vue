<template>
  <div class="home">
    
    <img class="beach_pic" alt="Photo de la plage de Saint-Anne" src="../assets/plage.jpeg">
    <div class="logo"><h1 class="two_rem">Chez <br/> Patricia et Joel</h1></div>
    <div class="text">
        <h2 class="two_rem">Maison en location saisonnière sur une île de rêve  </h2>
        <p>Découvrez la maison de vacance idéale pour votre séjour en martinique</p>
    </div>

    <div class="go_to_gallery">
        <p>Découvrez la maison de vacance idéale pour votre séjour en martinique</p>
        <button class="btn_style" @click="go_to_gallery">Découvrir la maison</button>
    </div>

    <p>La maison est située au sud de la Martinique</p>
    <p>Au plein coeur du bourg de Sainte-Anne, profitez de toutes les commodité et de notre belle plage à 5 min de marche à pied🚶🏻‍♀️</p>

    <div class="go_to_contact">
      <div class="caption">
        <p>Faite le pleins de souvenirs en réservant une maison qui vous plonge au coeur de la Martinique</p>
        <button class="btn_style">Je veux réserver</button>
      </div>
    </div>
    <div>
       <p>Venez profiter de l'air Martiniquais toute l'année!</p>
       <button class="btn_style btn_color_two" @click="go_to_agenda"> Je vérifie les dates de disponibilité!</button>

    </div>
    <h2>Les avis clients:</h2>
   


  
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Home',
  components: {
    
  },
  methods:{
    go_to_agenda(e){
      e.preventDefault();
      this.$router.push({path:'/Agenda'})
    }, 
    go_to_gallery(e){
      e.preventDefault();
      this.$router.push({path:'/Gallery'})
    },

  }
}
</script>
<style lang="scss" scoped>
.home{
  margin: 0%;
  width: 100%;
  margin-bottom: 200px;
  position: relative;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.beach_pic{
height: 200px;
overflow: hidden;
width: 100%;
object-fit: cover;
margin: 0%;
object-position: center;  
}
.logo{
 
  position: absolute;
  top: 100px;
  border-radius: 50%;
 background-color: skyblue;
 height: 200px;
 width: 200px;
 border:5px #fff solid;
 display: flex;
 justify-content: center;
 align-items: center;
 font-family: 'Dancing Script', cursive;

color: #fff;
}
.text{
  margin-top: 100px;
  font-weight: bold;
}
.two_rem{
   font-size: 2rem;
}

.go_to_gallery{
  position: relative;
  margin: 0%;
  width: 100%;
  height: 300px;
  background-image: url("../assets/photos.jpg");
  background-size: cover;
  background-position: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
   color: #fff;
  font-weight: bold;
  text-shadow: 1px 2px 2px black;
  font-size: 1.5rem;

}


.go_to_contact{
  position: relative;
  margin: 0%;
  width: 100%;
  height: 300px;
  background-image: url("../assets/souvenirs.jpg");
  background-size: cover;
  background-position: center;
  display: flex;
  align-items: center;

}

.caption{

  top:30px;
  left:0px;
  width: 47%;
  color: #fff;
  font-weight: bold;
  text-shadow: 1px 2px 2px black;
}

.btn_style{
  border-radius: 25px 25px 25px 25px ;
  height: 50px;
  background-color: palevioletred;
  color: #fff;
}
.btn_color_two{
background-color:skyblue ;
}
</style>