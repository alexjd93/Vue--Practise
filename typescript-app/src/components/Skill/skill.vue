<template lang="">
  <div class="skill">
    <h1 class="Skill_Title">My Strong Skills</h1>
    <div class="flex space-x-4">
      <div
        class="skill_box lg:w-1/2"
        v-for="(content, index) in SkillContentValue"
        v-bind:key="index"
      >
        <div class="skill_logo">logo</div>
        <div class="skill_box_description">
          <h4 class="text-center">{{ content.title }}</h4>
          <div class="h-40">
            {{ content.description }}
          </div>
        </div>
        <button>{{ content.button_primary }}</button>
      </div>
    </div>
  </div>
</template>
<script>
import { SkillContentValue } from "../../dummy_content/dummyData";
export default {
  name: "Skill_content",
  data() {
    return {
      SkillContentValue,
    };
  },
};
</script>
<style lang=""></style>
