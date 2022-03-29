<template lang="">
  <div class="content">
    <h2 class="text-3xl text-center mb-8">My Works</h2>
    <div
      class="grid grid-flow-row md:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 gap-10"
    >
      <div
        class="work_box"
        v-for="(content, index) in WorkContentValue"
        v-bind:key="index"
      >
        <div class="work_content">
          <h4>{{ content.title }}</h4>
          <div class="description">{{ content.description }}</div>
          <div class="">
            <div class="flex p-">
              <a
                class="bg-rose-200 w-1/2 p-5 text-center"
                :href="content.web_url"
              >
                {{ content.button_primary }}
              </a>
              <a class="bg-rose-200 w-1/2 p-5 ml-2 text-center">
                {{ content.button_secondary }}
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import { defineComponent } from 'vue';
import { WorkContentValue } from '../../dummy_content/dummyData';
export default defineComponent({
  name: 'WorkContent',
  data() {
    return {
      WorkContentValue,
    };
  },
});
</script>
<style lang=""></style>
