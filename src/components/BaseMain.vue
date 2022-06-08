<template>

    <main>
        <SelectInput/>
        <SectionAlbum/>

    </main>

</template>


<script>
import SelectInput from './SelectInput.vue';
import SectionAlbum from '../components/SectionAlbum.vue';

export default {
    name: 'BaseMain',
    components: {
        SelectInput,
        SectionAlbum,

    },

}
</script>

<style lang="scss" scoped>

    main{
        background-color: #1e2d3b;
    }

</style>