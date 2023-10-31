<script setup lang="ts">
import { 
  IonPage, 
  IonContent, 
  IonGrid, 
  IonIcon,
  IonCol,
  IonLabel,
  IonInput,
  IonRow,
  IonRippleEffect ,
  IonSelect, 
  IonSelectOption,
  IonText,
  IonNote
} from '@ionic/vue';
import { arrowBack, logoFacebook } from 'ionicons/icons'
</script>

<template>
  <ion-page>
    <ion-content :fullscreen="true">
      <ion-grid class="flex justify-center items-center h-full px-5 max-w-md min-w-fit">
        <ion-col>
          <ion-icon class="block text-lg" :icon="arrowBack" >
          </ion-icon>
          <ion-text class="block font-bold capitalize text-2xl">sign up</ion-text>
          <!-- email -->
          <ion-label class="block my-1 w-full">Email Address</ion-label>
          <ion-row class="flex-nowrap items-center border border-gray-600 rounded-md px-2">
            <ion-input class="text-sm legacy-input h-10" type="email" color="medium" shape="round" placeholder="Email Address"></ion-input>
          </ion-row>
          <!-- full name -->
          <ion-row>
            <ion-col class="pl-0">
              <ion-label class="block my-1 w-full">First Name</ion-label>
              <ion-row class="flex-nowrap items-center border border-gray-600 rounded-md px-2">
                <ion-input class="text-sm legacy-input h-10" type="text" color="medium" shape="round" placeholder="First Name"></ion-input>
              </ion-row>
            </ion-col>
            <ion-col class="pr-0">
              <ion-label class="block my-1 w-full">Last Name</ion-label>
              <ion-row class="flex-nowrap items-center border border-gray-600 rounded-md px-2">
                <ion-input class="text-sm legacy-input h-10" type="text" color="medium" shape="round" placeholder="Last Name"></ion-input>
              </ion-row>
            </ion-col>
          </ion-row>
          <!-- DOB -->
          <ion-label class="block my-1 w-full">Date of Birth(only for petsitters)</ion-label>
          <ion-row class="flex-nowrap items-center border border-gray-600 rounded-md px-2">
            <ion-input class="text-sm legacy-input h-10" type="text" color="medium" shape="round" placeholder="DD/MM/YYYY"></ion-input>
          </ion-row>
          <!-- phone -->
          <ion-label class="block my-1 w-full">Kraj</ion-label>
          <ion-row class="flex-nowrap items-center border border-gray-600 rounded-md px-2">
            <ion-select value="area_code" class="w-24 mr-1" style="min-height: 2rem;" justify="end">
              <ion-select-option value="apple">+866</ion-select-option>
              <ion-select-option value="banana">+1</ion-select-option>
              <ion-select-option value="orange">+44</ion-select-option>
            </ion-select>
            <ion-input class="text-sm legacy-input h-10 border-l border-gray-600" style="padding-left: 5px!important;" color="medium" shape="round" placeholder="DD/MM/YYYY"></ion-input>
          </ion-row>
          <!-- password -->
          <ion-label class="block my-1 w-full">Password</ion-label>
          <ion-row class="flex-nowrap items-center border border-gray-600 rounded-md px-2">
            <ion-input class="text-sm legacy-input h-10" type="password" color="medium" shape="round" placeholder="Password"></ion-input>
          </ion-row>
          <ion-note class="block my-3 text-sm text-center">by signing up you accenpt the <span>terms and conditions</span></ion-note>
          
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