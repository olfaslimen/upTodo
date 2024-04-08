<template>
  <div
    class="no-tasks"
  >
    <v-icon
      size="100"
      color="#E57373"
    >
      mdi-check
    </v-icon>
    <div class=""  ><h2 style="color:#E57373">Aucune tache trouvèe</h2> </div>
  </div>
</template>

<style lang="sass">
  .no-tasks
    position: absolute
    left: 50%
    top: 50%
    transform: translate(-50%, -50%)
    opacity: 0.5
</style>