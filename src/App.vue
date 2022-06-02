<script setup lang="ts">
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import AdInputVue from "./components/atoms/AdInput.vue";
import { reactive } from "vue";

const data = reactive({
  inputVal: "",
});
</script>

<template>
  <AdInputVue
    placeholder="Please enter your username"
    v-model="data.inputVal"
  />
  <p>Data of input is {{ data.inputVal }}</p>
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
