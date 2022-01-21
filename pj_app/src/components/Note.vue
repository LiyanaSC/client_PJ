<template>
    <div class="note">
        <p  class="name">{{ name }}</p>
        <p  class="title">{{ title }}</p>
        <p>{{ txt }}</p>
    </div>
</template>

<script>
export default {
  name: 'Note',
  props: {
      title: String,
       name: String,
    txt: String
  }
}
</script>

<style lang="scss" scoped>
.note{
    display: flex;
    flex-direction: column;
}
.name{
        font-family:'Dancing Script', cursive;
        font-size: 2rem;
        color: rgb(89, 0, 255);

}

.title{
    font-size: 1rem;
    font-weight: bold;
    margin: 0%;
}
</style>