<template>
  <main>
      <AppJumbotron />
      <AppInfoDrive />
      <AppInstructor />
  </main>
</template>

<script>
import AppJumbotron from "./main-components/AppJumbotron.vue";
import AppInfoDrive from "./main-components/AppInfoDrive.vue";
import AppInstructor from "./main-components/AppInstructor.vue"

export default {
    name: "AppMain",
    components: {
      AppJumbotron,
      AppInfoDrive,
      AppInstructor
    }
}
</script>

<style>

</style>