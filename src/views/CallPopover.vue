<template>
  <ion-page>   
    <ion-content class="ion-padding">
      <ion-button @click="openPopover">Process!</ion-button>
    </ion-content>
  </ion-page>
</template>

<script>
  import { IonButton, IonContent, IonPage, popoverController } from '@ionic/vue';
  import Popover from './HomePage.vue';

  export default{
    components: { IonButton, IonContent, IonPage },
    methods: {
      async openPopover(theEvent){
        const popover = await popoverController
        .create({
          component: Popover,
          event: theEvent,
          translucent: true
        })
        return popover.present();
      },
    },
  };
</script>