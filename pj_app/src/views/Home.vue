<template>
  <div class="home">
   
    <div class="text">
        <h2 class="two_rem">Maison en location saisonnière sur une île de rêve  </h2>
        <p>Située au sud de la Martinique dans la jolie commune de Sainte-Anne</p>
    </div>

    <div class="go_to_gallery">
        <p>Découvrez la maison de vacance idéale pour votre séjour</p>
        <button class="btn_style" @click="go_to_gallery">Découvrir la maison</button>
    </div>

    <p class="big_screen_size">
      Au plein coeur du bourg de Sainte-Anne, 
      <br/> profitez de toutes les commodité et de notre belle plage à 5 min de marche à pied🚶🏻‍♀️
      <br/>Patricia et Joel vous accueilleront dans une maison de vacance idéale de part
      <br/>sa position géographique qui vous offre le plaisir de profiter de la Plage🏖️
      <br/>que de sa proximité avec tout un tas de commodités!🍽️
      <br/>Ici le slogan c'est manger, nager🏊🏽‍♀️
    </p>

    <div class="go_to_contact">
      <div class="caption">
        <p>Faite le pleins de souvenirs en réservant une maison qui vous plonge au coeur de la Martinique</p>
        <button class="btn_style"  @click="go_to_contact">Je veux réserver</button>
      </div>
    </div>
    <div class="go_to_agenda">
       <p>Venez profiter de l'air Martiniquais toute l'année!</p>
       <button class="btn_style btn_color_two" @click="go_to_agenda"> Je vérifie les dates de disponibilité!</button>

    </div>
    <h2 class="customer">Les avis clients:</h2>
   


  
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
    go_to_contact(e){
      e.preventDefault();
      this.$router.push({path:'/Contact'})
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
      @media screen and (min-width: 900px) {
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: space-around;
  
    }
   
    
    
    
}

.text{
  font-weight: bold;
        margin-bottom: 50px;

     @media screen and (min-width: 900px) {
    width: 100%;
    & p{
      font-size: 1rem;
    }
    }
  
}
.two_rem{
   font-size: 2rem;
}

.go_to_gallery{
  position: relative;
  margin: 0%;
  width: 100%;
  height: 300px;
  background-image: url("../assets/go_to2.jpg");
  background-size: cover;
  background-position: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
   color: #fff;
  font-weight: bold;
  text-shadow: 1px 2px 2px gray;
  font-size: 1.5rem;
    margin-bottom: 50px;
    @media screen and (min-width: 900px) {
      
    margin-top: 50px;
    width: 40%;
    flex-direction: column;
    box-shadow: 1px 2px 2px gray;
    margin-bottom: 100Px;

    }

   

}


.go_to_contact{
  position: relative;
  margin: 0%;
  width: 100%;
  height: 300px;
  background-image: url("../assets/go_to.jpg");
  background-size: cover;
  background-position: center;
  display: flex;
  align-items: center;
    margin-top: 50px;
      margin-bottom: 50px;


   @media screen and (min-width: 900px) {
       background-attachment: fixed;
  background-image: url("../assets/go_to_hd.jpg");
    margin-top: 100px;
    width: 110%;
    flex-direction: column;
    box-shadow: 1px 2px 2px gray;
    margin-bottom: 100Px;
    order:6;
    align-items: start;
    justify-content: center;
    }

}
.go_to_agenda{
  margin-bottom: 50px;
@media screen and (min-width: 900px) {
      order:5;
  margin-bottom: 0px;
    }
}

.caption{

  top:30px;
  left:0px;
  width: 47%;
  color: #fff;
  font-weight: bold;
  text-shadow: 1px 2px 2px black;
  margin-left: 50px;
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
.big_screen_size{
@media screen and (min-width: 900px) {
     width: 50%;
  
    }
}
</style>