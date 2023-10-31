<script setup lang="ts">
import { IonPage, IonContent, IonImg, IonText, IonGrid } from '@ionic/vue';
import { useIonRouter } from '@ionic/vue';

import logo from '@/assets/imgs/logo.svg'

const ionRouter = useIonRouter();

setTimeout(() => {
  ionRouter.push('/login')
}, 3000);


</script>

<template>
  <ion-page>
    <ion-content :fullscreen="true">
      <ion-grid class="flex justify-center items-center h-full bg-gradient-to-b from-teal-400 to-yellow-200">
        <ion-img :src="logo" class="w-36 block responsive"></ion-img>
      </ion-grid>
    </ion-content>
  </ion-page>
</template>