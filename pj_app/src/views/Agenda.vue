<template>
    <div class="agenda">
        <div v-if="spinner" class="lds-dual-ring"></div>
        <h2 v-show="!spinner">L'agenda</h2>
        <div class="agenda__box">
            
            <iframe v-show="!spinner" src="https://calendar.google.com/calendar/embed?height=600&wkst=2&bgcolor=%23ffffff&ctz=America%2FMartinique&showTitle=0&showNav=1&showPrint=0&showCalendars=0&showTz=0&showTabs=0&showDate=1&src=2bf5lo91oohfrahdg8q8jje89s%40group.calendar.google.com&color=%23D81B60" style="border-width:0" width="95%" height="95%" frameborder="0" scrolling="no"></iframe>    


      </div>
    </div>
</template>

<script>
export default {
  components: {  },
   data(){
       return{
            spinner: true
       }
   },
   methods:{
      
   },
    mounted(){
      
   
      setTimeout(()=>{
        this.spinner=false
      },2000)
    }
    
}
</script>

<style lang="scss" scoped>
.agenda{
    //color: #fe6bb5;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin-bottom: 150px;
    &__box{
        width: 100%;
        height: 500px;
        @media screen and (min-width: 900px) {
            width: 80%;
            margin-top: 30px;;
  
    }
    }
}
.lds-dual-ring {
  display: inline-block;
  margin-top: 50px;
  width: 80px;
  height: 80px;
}
.lds-dual-ring:after {
  content: " ";
  display: block;
  width: 64px;
  height: 64px;
  margin: 8px;
  border-radius: 50%;
  border: 6px solid rgb(91, 182, 218) ;
  border-color: rgb(91, 182, 218)  transparent rgb(91, 182, 218)  transparent;
  animation: lds-dual-ring 1.2s linear infinite;
}
@keyframes lds-dual-ring {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}

</style>