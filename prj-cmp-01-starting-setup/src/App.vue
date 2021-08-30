<template>
<the-header title="Testing"> </the-header>
   <stored-resources :resources="storedResources"></stored-resources>

</template>

<script>
import StoredResources from './components/learning-res/StoredResources.vue';
import TheHeader from './components/layouts/TheHeader.vue';
export default {
components: {
    StoredResources,
    TheHeader,

},

    data() {
        return {
            storedResources: [
                {
                    id: 'project-inuse', 
                    title: 'Official Guide', 
                    description: 'Practise',
                    link: 'abc'
                },
                {
                    id: 'google',
                    title: 'Google ln',
                    description: 'Search engine',
                    link: 'https://google.com'
                }
            ]
        };
    },
    
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Varela+Round&display=swap');

* {
    box-sizing: border-box;
}

html {
    font-family: 'Varela Round', sans-serif;
}

body {
    margin: 0;
}

</style>