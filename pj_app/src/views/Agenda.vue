<template>
    <div class="agenda">
        <headerlogo/>
        <h2>L'agenda</h2>
        <div class="agenda__box">
            <iframe src="https://calendar.google.com/calendar/embed?height=600&wkst=2&bgcolor=%23ffffff&ctz=America%2FMartinique&showTitle=0&showNav=1&showPrint=0&showCalendars=0&showTz=0&showTabs=0&showDate=1&src=NG41amdwNmJsNjZtMGtlNWJhbnZqMGhybzBAZ3JvdXAuY2FsZW5kYXIuZ29vZ2xlLmNvbQ&color=%23D81B60" style="border-width:0" width="95%" height="95%" frameborder="0" scrolling="no"></iframe>    
           
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
.agenda{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    &__box{
        width: 100%;
        height: 500px;
    }
}
</style>