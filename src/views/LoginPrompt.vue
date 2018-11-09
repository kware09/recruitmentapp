<template>
<div class="w-custom mx-auto flex pt-5 justify-between">
  <div class="flex-1 bg-white shadow rounded p-5">
    <p class="text-lg">Register</p>
    <p class="text-grey-darker text-xs font-thin pt-3">Please use an email address we can contact you at, we will store your details for the next time you vist</p>
    <form class="bg-white px-8 pt-6 pb-8 mb-4">
    <div class="mb-4">
      <label class="block text-grey-darker text-sm font-bold mb-2" for="username">
        Email Address
      </label>
      <input class="shadow appearance-none border rounded w-full
      py-2 px-3 text-grey-darker leading-tight focus:outline-none focus:shadow-outline" id="username" type="text">
    </div>
    <div class="mb-4">
      <label class="block text-grey-darker text-sm font-bold mb-2" for="username">
        Forename
      </label>
      <input class="shadow appearance-none border rounded w-full py-2 px-3 text-grey-darker leading-tight focus:outline-none focus:shadow-outline" id="username" type="text">
    </div>
    <div class="mb-4">
      <label class="block text-grey-darker text-sm font-bold mb-2" for="username">
        Surname
      </label>
      <input class="shadow appearance-none border rounded w-full py-2 px-3 text-grey-darker leading-tight focus:outline-none focus:shadow-outline" id="username" type="text">
    </div>
    <div class="mb-6">
      <label class="block text-grey-darker text-sm font-bold mb-2" for="password">
        Password
      </label>
      <input class="shadow appearance-none border rounded w-full py-2 px-3 text-grey-darker leading-tight focus:outline-none focus:shadow-outline" id="password" type="password">
    </div>
    <div class="mb-6">
      <label class="block text-grey-darker text-sm font-bold mb-2" for="password">
        Confirm Password
      </label>
      <input class="shadow appearance-none border rounded w-full py-2 px-3 text-grey-darker mb-3 leading-tight focus:outline-none focus:shadow-outline" id="password" type="password">
    </div>
    <div class="flex items-center justify-between">
      <primary-button-link label="Register" route="/newapplication"></primary-button-link>
    </div>
  </form>
  </div>
  <div class="w-6"></div>
  <div class="flex-1 bg-white shadow rounded p-5">
    <p class="text-lg">Welcome Back</p>
    <p class="text-grey-darker text-xs font-thin pt-3">Please login we have your details so this should only take a minute</p>
    <form class="bg-white px-8 pt-6 pb-8 mb-4">
    <div class="mb-4">
      <label class="block text-grey-darker text-sm font-bold mb-2" for="username">
        Username
      </label>
      <input class="shadow appearance-none border rounded w-full py-2 px-3 text-grey-darker leading-tight focus:outline-none focus:shadow-outline" id="username" type="text">
    </div>
    <div class="mb-6">
      <label class="block text-grey-darker text-sm font-bold mb-2" for="password">
        Password
      </label>
      <input class="shadow appearance-none border rounded w-full py-2 px-3 text-grey-darker mb-3 leading-tight focus:outline-none focus:shadow-outline" id="password" type="password">
    </div>
    <div class="flex items-center justify-between">
      <primary-button-link label="Sign In" route="/newapplication"></primary-button-link>
      <a class="inline-block align-baseline font-bold text-sm text-teal hover:text-teal-darker" href="#">
        Forgot Password?
      </a>
    </div>
  </form>

  </div>
</div>
</template>
<script>
import PrimaryButtonLink from '@/components/PrimaryButtonLink.vue';

export default {
  name: 'LoginPrompt',
  components: {
    PrimaryButtonLink,
  },
};
</script>

<style scoped>
</style>
