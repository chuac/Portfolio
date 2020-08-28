<template>
    <div>
        <h1 class="section-header">Projects</h1>
        <project 
            v-for="project in projects" 
            v-bind:key="project.name" 
            v-bind:project="project" 
        ></project>
    </div>
</template>

<script>
import Project from './Project.vue'

export default {
    components: {
      'project': Project
    },
    data() {
        return {
            projects: [
                {
                    name: 'Waiting List',
                    description: 'A two-page app for a local business where staff can add customers and their desired game types to the wait list. The Display page would be open on a large TV for customers to view the dynamically updated waiting list.',
                    skills: ['HTML5', 'CSS3', 'JavaScript', 'ES6', 'Vue.js', 'Vuex', 'SpeechSynthesis'],
                    live_demo: 'https://waitlist.chuac.me/',
                    github: 'https://github.com/chuac/Waiting-List'
                },
                {
                    name: 'Test project',
                    description: '...',
                    live_demo: 'https://waitlist.chuac.me/',
                    github: 'https://github.com/chuac/Waiting-List'
                }
            ]
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
