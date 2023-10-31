<script setup lang="ts">
import { 
  IonPage, 
  IonText,
  IonInput,
  IonGrid,
  IonIcon,
  IonLabel,
  IonCol,
  IonRow,
  IonContent 
} from '@ionic/vue';
import { mailOutline, shieldCheckmarkOutline, logoFacebook } from "ionicons/icons"

</script>

<template>
  <ion-page>
    <ion-content :fullscreen="true">
      <ion-grid class="flex justify-center items-center h-full px-5 max-w-md min-w-fit">
        <ion-col>
          <ion-text class="block font-bold capitalize text-2xl">sign in</ion-text>

          <ion-text class="block">
            <span>Enter your details for sign in</span>
          </ion-text>

          <!-- email -->
          <ion-col>
            <ion-label class="block mb-2 w-full">Email Address</ion-label>
            <ion-row class="flex-nowrap items-center border border-gray-600 rounded-md px-2">
              <ion-icon :icon="mailOutline" size="large" class="text-gray-600 text-2xl mr-2">icon</ion-icon>
              <ion-input type="email" color="medium" shape="round" placeholder="Email Address"></ion-input>
            </ion-row>
          </ion-col>

          <!-- password -->
          <ion-col>
            <ion-label class="block mb-2 w-full">Password</ion-label>
            <ion-row class="flex-nowrap items-center border border-gray-600 rounded-md px-2">
              <ion-icon :icon="shieldCheckmarkOutline" size="large" class="text-gray-600 text-2xl mr-2">icon</ion-icon>
              <ion-input type="password" color="medium" shape="round" placeholder="Password"></ion-input>
            </ion-row>
          </ion-col>
          <ion-text class="relative -top-2 block w-full text-end cursor-pointer capitalize">forgot password?</ion-text>

          <ion-col class="block rounded-full text-center bg-green-500 text-white py-2 active:opacity-90">Sign Up</ion-col>
          <ion-col class="flex items-center">
            <ion-text class="flex-1 "></ion-text>
            <ion-text class="flex-1 h-0.5 bg-gray-300"></ion-text>
            <ion-text class="px-4">or</ion-text>
            <ion-text class="flex-1 h-0.5 bg-gray-300"></ion-text>
            <ion-text class="flex-1 "></ion-text>
          </ion-col>
          <ion-text class="relative block rounded-full text-center border border-gray-500 py-2 items-center">
            <ion-icon class="absolute inset-1.5 left-2 text-3xl text-blue-700" :icon="logoFacebook"></ion-icon>
            Login with Facebook
          </ion-text>
  
        </ion-col>
      </ion-grid>
    </ion-content>
  </ion-page>
</template>

<style scoped>
.page-center {
  display: flex;
  height: 100%;
  align-items: center;
  justify-content: center;
  padding-left: 15px;
  padding-right: 15px;
}
.input-container {
  flex-wrap: nowrap;
  padding: 0 8px;
  align-items: center;
  border: solid 1px #948989;
  border-radius: 5px;
}
.input-icon {
  font-size: 1.5rem;
  margin-right: 6px;
}
</style>