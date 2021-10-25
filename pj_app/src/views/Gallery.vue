<template>
    <section class="gallery">
        <headerlogo/>
        <img src="../assets/geo.svg" alt="icone de geolocalisation" style="height:50px">
        <p class="adress">8 cité des flamboyants <br/> 97227 Sainte-Anne</p>
        
        <h2>Les équipements:</h2>

         <ul>
          <li>1 salle à manger aménagée</li>
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
       <pics txt="Le salon" :url="require('@/assets/salon2.jpg')"/>
       <pics txt="La chambre orange" :url="require('@/assets/chambreorange.jpg')"/>
       <pics txt="La chambre verte" :url="require('@/assets/chambreverte.jpg')"/>
       <pics txt="La chambre bleu" :url="require('@/assets/Chambrebleu.jpg')"/>
      
       <pics txt="La cuisine" :url="require('@/assets/cuisine.jpg')" />
       <pics txt="La cuisine" :url="require('@/assets/cuisine2.jpg')"/>



       <pics txt="Plage de" :url="require('@/assets/plage2.jpeg')"/>
       <pics txt="Plage de" :url="require('@/assets/plage.jpeg')"/>
    </section>
</template>

<script>
import Headerlogo from '../components/Headerlogo.vue'
import Pics from '../components/Pics.vue'
export default {
  components: { Headerlogo, Pics },
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

</style>