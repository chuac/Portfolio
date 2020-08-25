<template>
    <div>
        <h1 class="section-header">Projects</h1>
        <project 
            v-for="project in projects" 
            :key="project.name" 
            :project="project" 
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
                    description: '...',
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
