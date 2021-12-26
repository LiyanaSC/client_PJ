<template>
    <section class="gallery">
        <a  href="https://www.google.com/maps/place/14°25'58.5%22N+60°52'54.2%22W/@14.432922,-60.8839069,967m/data=!3m1!1e3!4m5!3m4!1s0x0:0x2e7bbe0a60d172a6!8m2!3d14.432922!4d-60.8817182?hl=fr" target="_blank"><img src="../assets/geo.svg" alt="icone de geolocalisation" style="height:50px"></a>
       <a  href="https://www.google.com/maps/place/14°25'58.5%22N+60°52'54.2%22W/@14.432922,-60.8839069,967m/data=!3m1!1e3!4m5!3m4!1s0x0:0x2e7bbe0a60d172a6!8m2!3d14.432922!4d-60.8817182?hl=fr" target="_blank"> <p class="adress">8 cité des flamboyants <br/> 97227 Sainte-Anne</p></a>
        
        <h2>Les équipements:</h2>

         <ul>
          <li>1 salle à manger aménagée</li>
          <li>3 chambres avec espace de rangement</li>
          <li>1 cuisine équipée ouverte sur le salon</li>
          <li>1 salle de bain avec WC</li>
          <li>1 WC indépendant</li>
          <li>1 véranda aménagé (petit salon,table,hamac)</li>
          <li>1 seconde véranda aménagé (douche, 2 bains de soleil, évier, lave-linge) </li>
          <li>Places de parking</li>
          <li>La connexion internet pour partager vos bons moments est biensur gratuite!</li>
           
        </ul>

        <p>Située au bourg de Sainte-Anne, la maison vous offre toutes les commodités nécessaires à un bon séjour 😎 <br/>proximité avec la plage🏖️, les restaurants🍴, etc...</p>
       
       <h2>Les photos:</h2>
       <div class="pics_box">
                <pics txt="Le salon" :url="require('@/assets/salon2.jpg')"/>
            <pics txt="La chambre orange" :url="require('@/assets/chambreorange.jpg')"/>
            <pics txt="La chambre verte" :url="require('@/assets/chambreverte.jpg')"/>
            <pics txt="La chambre bleu" :url="require('@/assets/Chambrebleu.jpg')"/>
            
            <pics txt="La cuisine" :url="require('@/assets/cuisine.jpg')" />
            <pics txt="La cuisine" :url="require('@/assets/cuisine2.jpg')"/>



            <pics txt="Plage Anse Tonnoir" :url="require('@/assets/plage2.jpeg')"/>
            <pics txt="Plage Anse Tonnoir" :url="require('@/assets/plage.jpeg')"/>
       </div>

    </section>
</template>

<script>
import Pics from '../components/Pics.vue'
export default {
  components: { Pics },
    setup() {
        
    },
}
</script>

<style lang="scss" scoped>
.gallery{
    margin-bottom: 200px;
    display: flex;
    flex-direction: column;
    align-items: center;
}
.adress{
    font-size: 2rem;
    font-weight: bold;
}
ul{
    list-style: none;
}
.pics_box{
    width: 100%;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
}
a{
     text-decoration: none;
     color: black;
        &:hover{
        
            color: rgb(91, 182, 218);
        }
}
</style>