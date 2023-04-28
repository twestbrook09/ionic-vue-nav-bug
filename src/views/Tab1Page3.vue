<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-buttons>
          <ion-back-button></ion-back-button>
        </ion-buttons>
        <ion-title>Tab 1 Page 3</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Tab 1 Page 3</ion-title>
        </ion-toolbar>
      </ion-header>
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent, IonButtons, IonBackButton } from '@ionic/vue';

export default defineComponent({
  name: "Tab1Page3",
  components: {IonPage, IonHeader, IonToolbar, IonTitle, IonContent, IonButtons, IonBackButton},
  methods: {
    page3() {
      this.$router.push("/tabs/tab1/tab1page3");
    }
  }
});
</script>
