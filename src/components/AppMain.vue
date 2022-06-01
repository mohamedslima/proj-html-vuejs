<template>
  <main>
      <AppJumbotron />
      <AppInfoDrive />
  </main>
</template>

<script>
import AppJumbotron from "./main-components/AppJumbotron.vue";
import AppInfoDrive from "./main-components/AppInfoDrive.vue";

export default {
    name: "AppMain",
    components: {
      AppJumbotron,
      AppInfoDrive,
    }
}
</script>

<style>

</style>