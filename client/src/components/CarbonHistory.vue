<template lang="html">
  <div class="component" id="carbon-history">
    <h2>Your carbon history</h2>
    <chart :footprints="footprints" :categories="categories"/>
  </div>
</template>

<script>
import { eventBus } from '../main';
import Chart from './Chart.vue';

export default {
  name: "carbon-history",
  props: ["footprints", "categories"],
  components: {
    'chart': Chart
  }
}
</script>

<style lang="css" scoped>
.component {
  width: 80%;
  margin: 0 auto;
  background: rgba(255, 255, 255, 0.5);
  padding: 20px;
  margin-bottom: 40px;
}
</style>
