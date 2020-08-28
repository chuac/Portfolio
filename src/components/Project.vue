<template>
    <div class="project-container">
        
        <div class="project-image is-hidden-touch">
            <figure class="image is-5by4">
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
                <!-- <button>
                    Live Demo <i class="fas fa-external-link-alt"></i>
                </button> -->
                <a href="#" class="live-demo-button">
                    Live Demo <i class="fas fa-external-link-alt"></i>
                </a>
                <a href="#" class="view-source-button">
                    <i class="fab fa-github"></i> View Source
                </a>
                <button class="test-button button is-medium">
                    <span class="icon">
                        <i class="fab fa-github"></i>
                    </span>
                    <span>GitHub</span>
                </button>
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
