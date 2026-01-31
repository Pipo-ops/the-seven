<template>
  <div id="app">
    <div class="page">

      <!-- Reihe 1 -->
      <div class="row row-1">
        <BaseCard class="card-1">
          <CompanyCard/>
        </BaseCard>
        
      </div>

      <!-- Reihe 2 -->
      <div class="row row-2">
        <BaseCard class="card-2">
          <RevenueCard/>
        </BaseCard>
        <BaseCard class="card-3">
          <BreakdownCard/>
        </BaseCard>
      </div>

      <!-- Reihe 3 -->
      <div class="row row-3">
        <BaseCard class="card-4">
          <h1>Card 4</h1>
        </BaseCard>
        <BaseCard class="card-5">
          <h1>Card 5</h1>
        </BaseCard>
        <BaseCard class="card-6">
          <h1>Card 6</h1>
        </BaseCard>
      </div>

    </div>
  </div>
</template>

<script>
import BaseCard from "./components/BaseCard.vue";
import CompanyCard from "./components/CompanyCard.vue";
import RevenueCard from "./components/RevenueCard.vue";
import BreakdownCard from "./components/BreakdownCard.vue";

export default {
  name: "App",
  components: { BaseCard, CompanyCard, RevenueCard, BreakdownCard },
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

.page {
  padding: 100px;
  box-sizing: border-box;
  display: flex;
  flex-direction: column;
  gap: 32px;
}

.row {
  display: flex;
  gap: 32px;
}

.row-1 {
  justify-content: center;
}

.row-2,
.row-3 {
  justify-content: space-between;
}

.card-1{
  width: 100%;
}

.card-2,
.card-3 {
  flex: 1;
}

.card-4,
.card-5,
.card-6 {
  flex: 1;
}

</style>
