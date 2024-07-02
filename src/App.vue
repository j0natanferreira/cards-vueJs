<template>
  <div class="container">
    <SectionComponent />
  </div>
</template>

<script>
import SectionComponent from "./components/SectionComponent.vue";

export default {
  name: "App",
  components: {
    SectionComponent,
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Helvetica;
}

.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  background-color: #eeeeee;
  width: 100vw;
  height: 100vh;
}
</style>
