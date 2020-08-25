<template>
    <div class="project-container">
        
        <div class="project-image">

            <figure class="image is-5by4">
                <img src="https://bulma.io/images/placeholders/600x480.png">
            </figure>
        </div>

        <div class="project-content">
            <h3>{{ project.name }}</h3>
            <p>{{ project.description }}</p>
            <div class="project-skills">
                
            </div>
            <div class="project-links">

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
