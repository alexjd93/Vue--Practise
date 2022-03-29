<template>
  <Navigation />
  <Body />
  <Skill />
  <Work />
</template>

<script>
import Navigation from "./components/Navigation/navigation.vue";
import Body from "./components/Body/body.vue";
import Skill from "./components/Skill/skill.vue";
import Work from "./components/Work/work.vue";
export default {
  name: "App",
  components: { Navigation, Body, Skill, Work },
};
</script>

<style></style>
