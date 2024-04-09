<template>
  <ion-page>
    <ion-header :translucent="true">
      <ion-toolbar>
       <ion-searchbar animated="true" placeholder="Busqueda"></ion-searchbar>
        
      </ion-toolbar>
    </ion-header>

    <ion-content :Fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Busqueda</ion-title>
        </ion-toolbar>
      </ion-header>

      <div id="container">
        <ion-card>
    <ion-card-header>
      <ion-card-title color="success">Iniciar Sesion</ion-card-title>
      <ion-card-subtitle color="dark">o Registrarse</ion-card-subtitle>
    </ion-card-header>

    <ion-card-content>
      <ion-list>
    <ion-item>
      <ion-input label-placement="stacked" label="Email" placeholder="example@email.com">
        <ion-icon slot="start" :icon="lockClosed" aria-hidden="true"></ion-icon>
      </ion-input>
    </ion-item>
  </ion-list>

<ion-list>
<ion-item>
  <ion-input label-placement="stacked" label="Password" placeholder="Password" type="password">
        <ion-icon slot="start" :icon="lockClosed" aria-hidden="true"></ion-icon>
        <ion-button fill="clear" slot="end" aria-label="Show/hide">
          <ion-icon slot="icon-only" :icon="eye" aria-hidden="true"></ion-icon>
        </ion-button>
      </ion-input>
    </ion-item>
  </ion-list>
    </ion-card-content>

     <ion-button color="danger">Registrarse</ion-button>
        <ion-button color="success">Iniciar Sesion</ion-button>
  </ion-card>
        
       
      </div>
    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import { IonContent, IonHeader, IonPage, IonTitle, IonToolbar } from '@ionic/vue';
</script>

<style scoped>
#container {
  text-align: center;
  
  position: absolute;
  left: 0;
  right: 0;
  top: 50%;
  transform: translateY(-50%);
}

ion-card{
  font-size: 20px;
  margin-top: 3%;
}

ion-button{
  margin: 3%;
}
#container strong {
  font-size: 20px;
  line-height: 26px;
}

#container p {
  font-size: 16px;
  line-height: 50px;
  
  color: #8c8c8c;
  
  margin: 0;
}

#container a {
  text-decoration: none;
}


</style>
