<template>
  <form class="w-full">
  <div class="flex border-b border-b-2 border-teal py-2 ">
    <input class="appearance-none bg-transparent border-none w-full text-grey-darker mr-3 py-1 px-2 leading-tight focus:outline-none" type="text" placeholder="Search Jobs" aria-label="Search Jobs">
    <button class="flex-no-shrink bg-teal hover:bg-teal-dark border-teal hover:border-teal-dark text-sm border-4 text-white py-1 px-2 rounded mr-2" type="button">
      Search
    </button>
    <button class="flex-no-shrink border-transparent border-4 text-teal hover:text-teal-darker text-sm py-1 px-2 rounded" type="button">
      Login
    </button>
  </div>
</form>
</template>

<script>
export default {
  name: 'SearchBar',
};
</script>

