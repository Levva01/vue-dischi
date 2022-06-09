<template>

    <select name="album" id="genere" v-model="select.value">
        <option value="">All</option>
        <option value="Rock">Rock</option>
        <option value="Pop">Pop</option>
        <option value="Metal">Metal</option>
        <option value="Jazz">Jazz</option>

    </select>

</template>

<script>

import dataShared from '../../shared/dataShared.js';

export default {
    name: 'SelectInput',
    data(){
        return {
            dataShared
        }
    }
}
</script>

<style lang="scss" scoped>

    select{
        width: 6.25rem;
    }

</style>