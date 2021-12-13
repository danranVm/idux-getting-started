<script setup lang="ts">
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import HelloWorld from "./components/HelloWorld.vue";
</script>

<template>
  <IxDrawerProvider ref="drawerProviderRef">
    <IxModalProvider ref="modalProviderRef">
      <IxNotificationProvider>
        <IxMessageProvider>
          <HelloWorld />
        </IxMessageProvider>
      </IxNotificationProvider>
    </IxModalProvider>
  </IxDrawerProvider>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
