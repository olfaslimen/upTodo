<template>
    <v-btn
    @click="$store.commit('taskSorting')" 
    color="#E57373" 
    class="sortingBtn"
     >
        Priorité modifier
    </v-btn>
    </template>
<script>
export default{

}
</script>
<style>
.sortingBtn{
    position: fixed;
    bottom: 20px;
    left: 50%;
    transform: translateX(-50%);
}
</style>