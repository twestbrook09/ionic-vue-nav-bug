<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Tab 1 Page 0</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Tab 1 Page 0</ion-title>
        </ion-toolbar>
      </ion-header>
      <ion-button @click="page1">Page 1</ion-button>
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent, IonButton } from '@ionic/vue';
export default defineComponent({
  name: "Tab1Page",
  components: {IonPage, IonHeader, IonToolbar, IonTitle, IonContent, IonButton},
  methods: {
    page1() {
      this.$router.push("/tabs/tab1/page1");
    }
  }
});
</script>
