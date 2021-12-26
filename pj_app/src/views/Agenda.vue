<template>
    <div class="agenda">
        <h2>L'agenda</h2>
        <div class="agenda__box">
            <iframe src="https://calendar.google.com/calendar/embed?height=600&wkst=2&bgcolor=%23ffffff&ctz=America%2FMartinique&showTitle=0&showNav=1&showPrint=0&showCalendars=0&showTz=0&showTabs=0&showDate=1&src=2bf5lo91oohfrahdg8q8jje89s%40group.calendar.google.com&color=%23D81B60" style="border-width:0" width="95%" height="95%" frameborder="0" scrolling="no"></iframe>    


      </div>
    </div>
</template>

<script>
export default {
  components: {  },
    setup() {
        
    },
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
</style>