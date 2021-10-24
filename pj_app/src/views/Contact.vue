<template>
  <div class="about">
      <headerlogo/>
    <h2>Pour réserver:</h2>
    <div>
        <img class="" src="../assets/contact.svg" alt="icone d'appelle">
        <p>contactez nous par téléphone au: <br/>
            <a href="tel:+596696245899">0696245899</a> —
            <a href="tel:+596696459625">0696459625</a> —
            <a href="tel:+596696012181">0696012181</a>
        </p>
    </div>
    <div>
        <img style="height:50px" src="../assets/mail.svg" alt="icone de mail">
        <p>contactez nous par téléphone au: <br/>
            <a href="mailto:patricia.berenice@orange.fr">patricia.berenice@orange.fr</a>
        </p>
    </div>
    
  </div>
</template>

<script>
import Headerlogo from '../components/Headerlogo.vue'
export default {
  components: { Headerlogo },
    setup() {
        
    },
}
</script>

<style lang="scss" scoped>
.about{
    margin-bottom: 150px;
}
</style>
