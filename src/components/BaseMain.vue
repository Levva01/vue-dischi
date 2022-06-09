<template>

    <main>
        <SectionAlbum/>

    </main>

</template>


<script>
import SectionAlbum from '../components/SectionAlbum.vue';

export default {
    name: 'BaseMain',
    components: {
        SectionAlbum,

    },

}
</script>

<style lang="scss" scoped>

    main{
        background-color: #1e2d3b;
    }

</style>