<template>
  <section>
        <div class="albums-container">
            <CardMusic  v-for="music in musics" :key="music.id" :music="music"/>
        </div>
          
  </section>
</template>

<script>
import axios from 'axios';
import CardMusic from '../components/CardMusic.vue';
export default {
    name: 'SelectionAlbum',
    data() {
        return {
            musics: [],
        };
    },
    components: {
        CardMusic,
    },
    created() {
        axios.get('https://flynn.boolean.careers/exercises/api/array/music')
        .then((response) => {
            // handle success
            this.musics = response.data.response;
        })
        .catch((error) => {
            // handle error
            console.log(error);
        });
    }
}
</script>

<style lang="scss" scoped>


    section{
        background-color: #1e2d3b;
        display: flex;
        justify-content: center;


        .albums-container{
        width: 60%;
        padding: 3.125rem 0;
        display: flex;
        flex-wrap: wrap;
        gap: 1.875rem;
        }
    }

</style>