<template>
    <div class="outer" data-aos="flip-up">
        <img :src="require(`../assets/${img}.png`)" alt="NYT project">
            <div class="overlay">
                <h1>{{ description }}</h1>
                <a v-if="projectLink" :href="projectLink"  target="_blank">View Project</a>
                <a v-if="codeLink" :href="codeLink" target="_blank">View Code</a>
            </div>
    </div>    
</template>

<script>
export default {
    name: 'Project',
    props: [
        'img',
        'projectLink',
        'codeLink',
        'description'
    ],
}
</script>

<style scoped lang="stylus">

div.outer 
    position relative

div.overlay
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    height: 100%;
    width: 100%;
    opacity: 0;
    transition: .5s ease;
    background-color: #2C8C99;
    z-index 999
    display grid
    align-items center


    h1
        font-size 1.5rem 
        color white
    a
        color white
        text-decoration underline

.outer:hover .overlay
        opacity: .95;
    


</style>
