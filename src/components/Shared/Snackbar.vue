<template>
  <v-snackbar
    v-model="$store.state.snackbar.show"
    color="black"
    width="100%"
  >

    {{ $store.state.snackbar.text }}

    <template v-slot:action="{ attrs }">
      <v-btn
        @click="$store.commit('hideSnackbar')"
        text
        v-bind="attrs"
        color="#E57373"
      >
     
        Fermer
      </v-btn>
    </template>
  </v-snackbar>
</template>

<script>
export default {

}
</script>

<style>

</style>