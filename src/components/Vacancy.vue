<template>
    <router-link tag="div" to="/about"><div class="w-full mt-3 p-5 border-grey-ligher bg-white rounded-lg shadow border flex hover:bg-grey-lightest hover:shadow-md hover: cursor-pointer">
        <div>
            <p class="text-lg">{{jobTitle}}</p>
            <p class="text-sm text-grey-darker">{{location}}</p>
        </div>
    </div></router-link>
</template>

<script>
    export default {
        name: "Vacncy",
        props: {
            jobTitle: {
                type: String
            },
            location: {
                type: String
            }
            
        },
    }
</script>

<style scoped>
a {text-decoration: none;}

</style>