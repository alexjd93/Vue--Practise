<template>
  <div class="container mx-auto">
    <Navigation :navigation="navigationValue" />
    <Body />
    <Skill />
    <Work />
  </div>
</template>

<script>
import Navigation from "./components/Navigation/navigation.vue";
import Body from "./components/Body/body.vue";
import Skill from "./components/Skill/skill.vue";
import Work from "./components/Work/work.vue";
export default {
  name: "App",
  components: { Navigation, Body, Skill, Work },
  data() {
    return {
      navigationValue: [
        {
          Menu: "Home",
        },
        {
          Menu: "Project",
        },
        {
          Menu: "Skills",
        },
        {
          Menu: "Contact",
        },
      ],
    };
  },
};
</script>

<style></style>
