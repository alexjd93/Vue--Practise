<template>
  <div class="flex navigation px-8">
    <div class="navbar_logo">Alex Website</div>
    <ul
      v-for="(content, index) in navigationValue"
      v-bind:key="index"
      class="flex"
    >
      <li>content</li>
    </ul>
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
