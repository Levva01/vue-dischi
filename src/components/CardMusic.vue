<template>
  <div class="music">
      <img :src="music.poster" :alt="music.title">
      <h5>{{music.title}}</h5>
      <div>{{music.author}}</div>
      <div><strong>{{music.year}}</strong></div>
  </div>
</template>

<script>
export default {
    name: 'CardMusic',
    props: {
        music: Object,
    }
}
</script>

<style lang="scss" scoped>
.music {
    padding-top: 1.25rem;
    width: calc(100% / 5 - 30px);   
    height: 15.625rem;    
    background-color: #2e3a46;
    text-align: center;
    img {
        width: 6.25rem;
        height: 6.25rem;
        margin-bottom: 20px;
    }

    h5{
        color: white;
        overflow-wrap: break-word;
        text-transform: uppercase;
        font-size: .9375rem;
    }

    div{
        color: gray;
    }
}
</style>