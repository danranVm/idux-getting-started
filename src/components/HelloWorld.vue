<script setup lang="ts">
import { version } from "@idux/components/version";
import { useMessage } from "@idux/components/message";

const { info } = useMessage();
const onClick = () => info("Hello @idux");
</script>

<template>
  <h1>Hello @idux: {{ version }}</h1>
  <p>
    <IxButton mode="primary" @click="onClick">Say Hello</IxButton>
  </p>
  <p>
    See
    <a href="https://idux.site" target="_blank"> idux.site </a>
    for more information.
  </p>
</template>

<style scoped>
p {
  margin: 1em;
}
a {
  color: #1c6eff;
}
</style>
