<template>
    <div class="project-container">
        
        <div class="project-image is-hidden-touch">
            <figure class="image is-square">
                <img src="https://bulma.io/images/placeholders/600x480.png">
            </figure>
        </div>

        <div class="project-content">
            <h2 class="project-name">{{ project.name }}</h2>
            <p class="project-description">{{ project.description }}</p>
            <div class="project-skills">
                <span class="project-skill" v-for="skill in project.skills" v-bind:key="skill">
                    {{ skill }}
                </span>
            </div>
            <div class="project-links">
                <!-- <a href="#" class="live-demo-button">
                    Live Demo <i class="fas fa-external-link-alt"></i>
                </a> -->
                <a 
                    v-bind:href="project.live_demo_url" 
                    target="_blank" 
                    class="live-demo-button button"
                >
                    <span>Live Demo</span>
                    <span class="icon">
                        <i class="fas fa-external-link-alt"></i>
                    </span>
                </a>
                <a 
                    v-bind:href="project.github_url" 
                    target="_blank" 
                    class="view-source-button button"
                >
                    <span class="icon">
                        <i class="fab fa-github"></i>
                    </span>
                    <span>View Source</span>
                </a>
            </div>
        </div>

    </div>
</template>

<script>
export default {
    props: {
        project: Object
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
