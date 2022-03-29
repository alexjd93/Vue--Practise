<template lang="">
  <div class="my-50">
    <h2 class="text-3xl text-center">My Strong Skills</h2>
    <div class="md:flex md:flex-row justify-between">
      <div
        class="lg:w-1/4 p-8"
        v-for="(content, index) in SkillContentValue"
        v-bind:key="index"
      >
        <div class="skill_logo">logo</div>
        <div class="skill_box_description">
          <h4 class="text-center py-2">{{ content.title }}</h4>
          <div class="h-40">
            {{ content.description }}
          </div>
        </div>
        <div class="flex flex-row">
          <button>{{ content.button_primary }}</button>
          <button>{{ content.button_secondary }}</button>
        </div>
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
