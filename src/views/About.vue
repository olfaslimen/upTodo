<template>
  <div>
    <div class="ma-2 pa-2 mb-auto">
     
    <h1 class="text-center font-weight-black text-h2 ma-2 pa-2 mb-auto">Qu'est-ce que upTodo ?</h1>
    <p class="text-center ma-2 pa-2 mb-auto">
      upTodo est une application de gestion des tâches simple et efficace, conçue pour vous aider à planifier, suivre et accomplir vos tâches quotidiennes avec facilité. Que ce soit pour votre travail, vos études ou vos projets personnels, upTodo vous permet de rester organisé et concentré sur ce qui compte vraiment.    </p>
     </div>
      <template>
  <v-icon icon="home" />
</template>
<v-row align="center" justify="center">
    <v-col cols="auto">
      <v-card
        class="mx-auto"
        max-width="344"
     
      >
      
      
      <v-card-title>
        <v-icon
        color="success"
      >
        mdi-plus
      </v-icon> 
        Ajouter
            </v-card-title>
          
        <v-card-text>Créez rapidement de nouvelles tâches en spécifiant un titre et une date prévue pour leur réalisation.</v-card-text>
      </v-card>
    </v-col>

    <v-col cols="auto">
      <v-card
        class="mx-auto"
        max-width="344"
     
      >
      <v-card-title>
        <v-icon
        color="error"
      >
        mdi-delete
      </v-icon> 
        Supprimer
      
      </v-card-title>
        
        <v-card-text>Effacez les tâches terminées ou celles qui ne sont plus pertinentes en un seul clic pour maintenir votre liste de tâches propre et à jour.</v-card-text>
      </v-card>
    </v-col>

    <v-col cols="auto">
      <v-card
        class="mx-auto"
        max-width="400"
     
      >
      <v-card-title>
        <v-icon
        color="#01579B"
      >
        mdi-pencil
      </v-icon> 
        Modifier
      </v-card-title>
        <v-card-text>Besoin de changer le titre d'une tâche ou sa date prévue ? Pas de problème ! upTodo vous permet de modifier facilement vos tâches pour refléter vos besoins actuels.</v-card-text>
      </v-card>
    </v-col>

    <v-col cols="auto">
      <v-card
        class="mx-auto"
        max-width="344"
      >
      <v-card-title>
        <v-icon
        color="#9C27B0"
      >
        mdi-magnify
      </v-icon> 
        Rechercher
      
      </v-card-title>
       
        <v-card-text> Utilisez la fonction de recherche pour trouver rapidement une tâche spécifique en saisissant simplement son titre. Plus besoin de parcourir toute votre liste !</v-card-text>
      </v-card>
    </v-col>
  </v-row>
</div>
</template>


