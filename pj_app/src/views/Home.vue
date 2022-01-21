<template>
  <div class="home">
   
    <div class="text">
        <h2 class="two_rem">Maison en location saisonnière sur une île de rêve  </h2>
        <p>Située au sud de la Martinique dans la jolie commune de Sainte-Anne</p>
    </div>

    <div class="first_deco"> 
    </div>

    <div class="big_screen_size">
     <h3>Au plein coeur du bourg de Sainte-Anne</h3> 
      <h4>🏠 Logement entier</h4>
      <p>  
        <br/>Patricia et Joel vous accueilleront dans une maison de vacance idéale de part
        <br/>sa position géographique qui vous offre le plaisir de profiter de la Plage🏖️
      </p>

      <h4>📍 Idéalement situé</h4>
      <p>
      <br/> profitez de toutes les commodités et de notre belle plage à 5 min de marche à pied🚶🏻‍♀️
    
      <br/>que de sa proximité avec tout un tas de commodités!🍽️
      <br/>Ici le slogan c'est manger, nager🏊🏽‍♀️
      </p>

     
      
    </div>

  
    <div class="revert_small_screen">

            <div class="text_beside_deco">
            <p>Découvrez la maison de vacance idéale pour votre séjour</p>
              <button class="btn_style" @click="go_to_gallery">Découvrir la maison</button>
          </div>

          <div class="second_deco"> 
    </div>
    </div>

      <div class="third_deco"> 
       </div>

      <div class="text_beside_deco">
        <h3>Venez profiter de l'air Martiniquais toute l'année!</h3>
        <button class="btn_style btn_color_two" @click="go_to_agenda"> Je vérifie les dates de disponibilité!</button>

      </div>
    
    

        <div class="clients">
     <h2 class="customer">Nos avis clients:</h2> 
      <note name="Liyana" title="Un coin de Paradis" txt="Le site ne reflète même pas le confort et le bien être dont on bénéficie dans ce petit coin de paradis, j'ai passé un séjour (Trop court!) et que ce soit la douche extérieur trop pratique après la plage, le hamac, la douche à l'italienne, la proximité de tout, etc... On oublie le COVID, on est serein! On a tout à quelque pas. Vraiment un très grand plaisir! J'ai adoré, j'y reviendrai. Merci à Patricia et Joël des personnes très gentilles." />
  
    </div>

    <div class="go_to_contact">
      <div class="caption">
        <p>Faites le pleins de souvenirs en réservant une maison qui vous plonge au coeur de la Martinique</p>
        <button class="btn_style"  @click="go_to_contact">Je veux réserver</button>
      </div>
    </div>


    
    <div class="go_to_agenda">
      <div>
        <h2>Tarifs:</h2>
        <p>
          <br/> 1 chambre: weekend 200€ / semaine 350€
          <br/> 2 chambres: weekend 325€ / semaine 500€
          <br/> 3 chambres: weekend 400€ / semaine 700€
      
        </p>
      </div>


    </div>

    

 

  </div>
</template>

<script>
import Note from '../components/Note.vue';
// @ is an alias to /src

export default {
  name: 'Home',
  components: {
    Note
    
    
  },
  methods:{
    go_to_agenda(e){
      e.preventDefault();
      this.$router.push({path:'/Agenda'})
       window.scrollTo(0,0);
    }, 
    go_to_gallery(e){
      e.preventDefault();
      this.$router.push({path:'/Gallery'})
       window.scrollTo(0,0);
    },
    go_to_contact(e){
      e.preventDefault();
      this.$router.push({path:'/Contact'})
       window.scrollTo(0,0);
    },

  },

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

.first_deco{
  margin: 0%;
  height: 400px;
  width: 100%;
  background-image: url("../assets/hamac1.jpg");
  background-size: cover;
  background-position: center;
  font-weight: bold;
  text-shadow: 1px 2px 2px gray;

    @media screen and (min-width: 900px) {
      
    margin-top: 50px;
    height: 400px;
    width: 50%;
    flex-direction: column;

    }
}
.revert_small_screen{
margin: 0%;
padding:0%;
width: 100%;
display: flex;
flex-direction: column-reverse;

    @media screen and (min-width: 900px) {
      
   
    flex-direction: row;

    }
}
.second_deco{
   margin: 0%;
  height: 400px;
  width: 100%;
  background-image: url("../assets/go_to2.jpg");
  background-size: cover;
  background-position: center;
  font-weight: bold;
  text-shadow: 1px 2px 2px gray;

    @media screen and (min-width: 900px) {
      
  
    height: 400px;
    width: 50%;
    flex-direction: column;

    }
}
.third_deco{
 margin: 0%;
  height: 400px;
  width: 100%;
  background-image: url("../assets/plage3.jpg");
  background-size: cover;
  background-position: center;
  font-weight: bold;
  text-shadow: 1px 2px 2px gray;

    @media screen and (min-width: 900px) {
      
  
    height: 400px;
    width: 50%;
    flex-direction: column;

    }
}
.text_beside_deco{
  width: 100%;
  display: flex;
  justify-content: center;
     flex-direction: column;
    align-items: center;
    margin-bottom: 50px;

   @media screen and (min-width: 900px) {
      
  
    height: 400px;
    max-width: 50%;
 margin-bottom: 0px;

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
  
    align-items: start;
    justify-content: center;
    }

}
.go_to_agenda{
  margin-bottom: 50px;
@media screen and (min-width: 900px) {
  width: 100%;
display: flex;
justify-content: space-around;
  margin-bottom: 0px;
  align-items: center;
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


.btn_color_two{
background-color:rgb(91, 182, 218) ;
}
.clients{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
   @media screen and (min-width: 900px) {
      
   
    flex-direction: column-reverse;

    }
}
.customer{
    @media screen and (min-width: 900px) {
     
      width: 90%;
      margin-top: 100px;
  
    }

}
.big_screen_size{
@media screen and (min-width: 900px) {
  width: 50%;
  margin-bottom: 30px;
  text-align: left;
  box-sizing: border-box;
  padding-left: 50px;
  display: flex;
  flex-direction: column;
  & :nth-child(n){
    margin:0%;
  }
  & :nth-child(1){
    margin-bottom: 20px;
  }
  & :nth-child(3){
    margin-bottom: 20px;
  }
  & :nth-child(5){
    margin-bottom: 20px;
  }
      }
}
</style>