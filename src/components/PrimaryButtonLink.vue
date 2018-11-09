<template>
    <router-link v-bind:to="route" tag="button" class="flex-no-shrink bg-teal hover:bg-teal-dark border-teal hover:border-teal-dark text-sm border-4 text-white py-1 px-2 rounded"
                type="button">{{label}}</router-link>
</template>

<script>
export default {
  name: 'PrimaryButtonLink',
  props: {
    label: {
      type: String,
    },
    route: {
      type: String,
    },

  },
};
</script>

<style scoped>
a {
  text-decoration: none;
}
</style>
