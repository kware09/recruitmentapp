<template>
  <div class="md:w-custom sm:w-4/5 m-auto pt-5 ">
    <search-bar/>
    <vacancy job-title="Software Developer" location="Airport Busniess Park, Dublin"/>
    <vacancy job-title="Business Analyst" location="Airport Busniess Park, Dublin"/>
    <vacancy job-title="Project Manger" location="Airport Busniess Park, Dublin"/>
   </div>
</template>

<script>
// @ is an alias to /src
import SearchBar from '@/components/SearchBar.vue';
import Vacancy from '@/components/Vacancy.vue';

export default {
  name: 'home',
  components: {
    SearchBar,
    Vacancy,
  },
};
</script>
