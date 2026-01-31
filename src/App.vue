<template>
  <div id="app">
    <div class="page">
      <BaseCard>
        <h1>Hallo BaseCard 👋</h1>
      </BaseCard>
    </div>
  </div>
</template>

<script>
import BaseCard from "./components/BaseCard.vue";

export default {
  name: "App",
  components: { BaseCard },
};
</script>

<style>
html,
body {
  margin: 0;
  height: 100%;
}

#app {
  min-height: 100vh;
  width: 100%;
  background: radial-gradient(71.11% 100% at 50% 0%, #020204 14.6%, #011F35 100%);
}

/* Hier Padding statt auf body */
.page {
  padding: 100px;
  box-sizing: border-box; /* wichtig */
}
</style>
