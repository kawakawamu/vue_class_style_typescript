<template>
  <div id="app" class="app__wrapper">
    <CountNumber />
    <CountNumberExtend />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import CountNumber from "./components/CountNumber.vue";
import CountNumberExtend from "./components/CountNumberExtend.vue";

@Component({
  components: {
    CountNumber,
    CountNumberExtend,
  },
})
export default class App extends Vue {}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.app__wrapper {
  display: flex;
  justify-content: center;
}
</style>
