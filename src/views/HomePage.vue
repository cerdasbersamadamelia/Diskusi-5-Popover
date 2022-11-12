<template>
  <ion-content class="ion-padding">
    <ul>
      <li>NIM: 041643527</li>
      <li>Nama: Damelia</li>
      <li>UPBJJ: Jakarta</li>
    </ul>
  </ion-content>
</template>

<script>
  import { IonContent } from '@ionic/vue';
  import { defineComponent } from 'vue';

  export default defineComponent({
    name: 'HomePage',
    components: { IonContent }
  });
</script>