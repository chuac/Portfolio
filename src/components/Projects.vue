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
                    description: `
                            A local business was using a spreadsheet to show customers in a queue. It was simply mirrored onto a second display and staff vocally called out for customers.
                            <br><br>
                            I created a two-page solution where staff can add customers and control the queue on one page. The "Display" page would be open on a large TV for customers to view the dynamically updated waiting list. Also features Text-to-Speech at a click of a button. 
                            <br><br>
                            This web app is used by a team of five staff members serving hundreds of customers a night.
                        `,
                    skills: ['HTML5', 'CSS3', 'JavaScript', 'ES6', 'Vue.js', 'Vuex', 'SpeechSynthesis'],
                    live_demo_url: 'https://waitlist.chuac.me/',
                    github_url: 'https://github.com/chuac/Waiting-List'
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
