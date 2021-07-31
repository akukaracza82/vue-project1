<template>
    <ul>
        <learning-resource v-for="res in storedResources" :key="res.id" :title="res.title" :description="res.description" :link="res.link"></learning-resource>
    </ul>
</template>

<script>
import LearningResource from './components/learning-resources/LearningResource.vue'

export default {
    components: { 
        LearningResource 
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