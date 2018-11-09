/*global marked*/
<template>
    <div class="md:w-custom mx-auto shadow-md mb-10 rounded-lg mt-5">
        <div class="w-full bg-teal h-1 sticky pin-t"></div>
        <img class="w-full h-54 overflow-hidden" src="@/assets/ba.jpg">
        <div class="flex justify-between w-full p-5 sticky pin-t bg-white border-grey border-b m-0">
            <div>
                <p class="text-lg">Software Developer</p>
                <p class="text-sm text-grey-darker">Software Developer</p>
            </div>
            <primary-button-link label="Apply" route="/loginprompt"></primary-button-link>
        </div>
        <div class="w-full bg-white p-5">
            <div v-html="compiledMarkdown"></div>
            <div class="w-full flex justify-center mt-10">
                <router-link to="/" tag="button" class="flex-no-shrink bg-grey hover:bg-grey-dark border-grey hover:border-grey-dark text-sm border-4 text-white py-1 px-2 rounded align-middle"
                    type="button">Back to Jobs</router-link>
            </div>
        </div>
    </div>
</template>
<script>
import markdown from '@/assets/data/data.json';
import PrimaryButtonLink from '@/components/PrimaryButtonLink.vue';

export default {
  name: 'About',
  data() {
    return {
      input: '# hello',
    };
  },
  computed: {
    compiledMarkdown() {
      return marked(unescape(markdown.markdown), { sanitize: true });
    },
  },
  components: {
    PrimaryButtonLink,
  },
};
</script>

<style scoped>
</style>
