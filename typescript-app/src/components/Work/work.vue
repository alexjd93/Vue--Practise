<template lang="">
  <div class="work">
    <h1 class="Skill_Title">My Works</h1>
    <div class="flex space-x-4">
      <div
        class="work_box"
        v-for="(content, index) in WorkContentValue"
        v-bind:key="index"
      >
        <div class="work_content">
          <h4>{{ content.title }}</h4>
          <div class="description">{{ content.description }}</div>
          <div class="work_button_box flex">
            <button>{{ content.button_primary }}</button>
            <button>{{ content.button_secondary }}</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import { defineComponent } from "vue";
import { WorkContentValue } from "../../dummy_content/dummyData";
export default defineComponent({
  name: "WorkContent",
  data() {
    return {
      WorkContentValue,
    };
  },
});
</script>
<style lang=""></style>
