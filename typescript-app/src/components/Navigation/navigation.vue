<template>
  <div class="p-4">
    <div class="md:flex md:flex-row md:justify-between text-center">
      <div class="navbar_logo">Alex Website</div>
      <div>
        <a
          v-for="(content, index) in navigation"
          v-bind:key="index"
          class="p-4 hover:text-purple-600"
          >{{ content.Menu }}</a
        >
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Navigation_tag",
  components: {},
  props: {
    navigation: Array,
  },
};
</script>
