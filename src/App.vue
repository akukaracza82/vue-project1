<template>
    <the-header title="Remember Me"></the-header>
    <stored-resources :resources="storedResources"></stored-resources>
</template>

<script>
import StoredResources from './components/learning-resources/StoredResources.vue'
import TheHeader from './components/layouts/TheHeader.vue'

export default {
    components: { 
        StoredResources,
        TheHeader,
        },
    data() {
        return {
            storedResources: [
                {
                    id: 'guide1',
                    title: 'official guide 1',
                    description: 'description of the official guide 1',
                    link: 'https://vuejs.org'
                },
                 {
                    id: 'guide12',
                    title: 'official guide 12',
                    description: 'description of the official guide 12',
                    link: 'https://google.com'
                },
            ]
        }
    }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

* {
  box-sizing: border-box;
}

html {
  font-family: 'Roboto', sans-serif;
}

body {
  margin: 0;
}
</style>