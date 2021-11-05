<template>
    <header class="header">
         <div class="beach_pic"></div>
         <div class="logo" @click="go_back_home"><h1 class="two_rem">Chez <br/> Patricia et Joel</h1></div>
    </header>
</template>

<script>
export default {
  name: 'Headerlogo',
  methods:{
    go_back_home(){
      this.$router.push({path:'/'})
    }
  }
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
    background-image: url("../assets/plage3.jpg");
background-position: bottom;
background-size: cover;
width: 100%;
object-fit: cover;
margin: 0%;
object-position: center; 
       background-attachment: fixed;

  @media screen and (min-width: 900px) {
        background-image: url("../assets/plage3_hd.jpg");

    background-size: cover;
    background-position: center;
    background-attachment: fixed;
        width: 100%;
    height: 300px;

  }

}
.logo{
 
  position: absolute;
  top: 100px;
  border-radius: 50%;
 background-color: rgb(91, 182, 218);
 height: 200px;
 width: 200px;
 border:5px #fff solid;
 display: flex;
 justify-content: center;
 align-items: center;
 font-family: 'Dancing Script', cursive;
  color: #fff;
   @media screen and (min-width: 900px) {
    top:200px

  }
}
.two_rem{
   font-size: 2rem;
}
</style>
