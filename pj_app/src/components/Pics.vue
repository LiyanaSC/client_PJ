<template>
    <div class="shadow">
        <img class="pic" :src="url" :alt="txt">
        <p class="txt">{{ txt }}</p>

    </div>
</template>

<script>
export default {
  name: 'Pics',
  props: {
      url: String,
    txt: String
  }
}
</script>

<style lang="scss" scoped>
.shadow{
    box-shadow: 2px 2px 10px gray;
    height: 600px;
    width: 80%;
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;
    margin: 15px;
     @media screen and (min-width: 900px) {
        width: 25%;
  
    }
}
.pic{
    width: 90%;
    height: 70%;
    object-fit: cover;
    object-position: bottom;  
   

}
.txt{
    font-family:'Dancing Script', cursive;
    font-size: 2rem;
    margin: 0%;
}
</style>