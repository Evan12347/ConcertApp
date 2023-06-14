<script setup lang="ts">
import { IonPage, IonContent, IonInput, IonButton, IonImg } from '@ionic/vue';
import { ref } from 'vue';
const username = ref('');
const password = ref('');
</script>

<template>
  <ion-page>
    <ion-content :fullscreen="true">
      <div>
        <form>
          <ion-img
              src="https://img.freepik.com/photos-gratuite/vue-arriere-foule-fans-regardant-performances-direct-concert-musique-nuit-espace-copie_637285-544.jpg?w=2000"
              style="width: 50%;
             margin: auto;
             padding: 1rem">
          </ion-img>
          <ion-item>
            <ion-label position="floating">Nom d'utilisateur</ion-label>
            <ion-input
                type="text"
                fill="outline"
                v-model="username"
                required
            ></ion-input>
          </ion-item>
          <ion-item>
            <ion-label position="floating">Mot de passe</ion-label>
            <ion-input
                type="password"
                fill="outline"
                v-model="password"
                required
            ></ion-input>
          </ion-item>
          <ion-item>
            <ion-label>Administrateur</ion-label>
            <ion-checkbox fill="outline"></ion-checkbox>
          </ion-item>
          <ion-button type="submit">Inscription</ion-button>
        </form>
      </div>
    </ion-content>
  </ion-page>
</template>