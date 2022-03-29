<template lang="">
  <div class="my-50 content">
    <h2 class="text-3xl text-center mb-8">My Strong Skills</h2>
    <div
      class="grid grid-flow-row md:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 gap-10"
    >
      <div
        class="p-8"
        v-for="(content, index) in SkillContentValue"
        v-bind:key="index"
      >
        <div class="bg-rose-200 rounded-lg">
          <div class="text-center w-2/5 m-auto">
            <img src="../../assets/java.png" v-bind:alt="pic" />
          </div>

          <div class="skill_box_description p-4 text-center">
            <h4 class="text-center py-2">{{ content.title }}</h4>
            <div class="h-20">
              {{ content.description }}
            </div>
          </div>
          <div class="flex flex-row mx-auto justify-center p-4">
            <a
              class="bg-gradient-to-r from-red-600 to-pink-500 rounded-full py-3 px-5 text-gray-50 uppercase"
              >{{ content.button_primary }}</a
            >
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import { SkillContentValue } from '../../dummy_content/dummyData';
export default {
  name: 'Skill_content',
  data() {
    return {
      SkillContentValue,
    };
  },
};
</script>
<style lang=""></style>
