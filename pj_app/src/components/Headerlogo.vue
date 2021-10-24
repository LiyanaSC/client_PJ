<template>
    <header class="header">
         <img class="beach_pic" alt="Photo de la plage de Saint-Anne" src="../assets/plage.jpeg">
         <div class="logo"><h1 class="two_rem">Chez <br/> Patricia et Joel</h1></div>
    </header>
</template>

<script>
export default {
  name: 'Headerlogo',

}
</script>

<style lang="scss" scoped>
.header{
  margin: 0%;
  width: 100%;
  position: relative;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin-bottom: 150px;
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
</style>
