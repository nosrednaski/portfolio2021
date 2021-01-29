<template>
    <div class="container">
        <h1 data-aos="flip-up">Current</h1>
        <div class="grid">
            <Project v-for="project in current" :img="project.img" :projectLink="project.projectLink" :codeLink="project.codeLink" :description="project.description" :key="project.img"/>
        </div>

        <h1 data-aos="flip-up">Capital One</h1>
        <div class="grid">
            <Project v-for="project in cap1" :img="project.img" :projectLink="project.projectLink" :codeLink="project.codeLink" :description="project.description" :key="project.img"/>
        </div>

        <h1 data-aos="flip-up">Bootcamp</h1>
        <div class="grid four">
            <Project v-for="project in projects" :img="project.img" :projectLink="project.projectLink" :codeLink="project.codeLink" :description="project.description" :key="project.img"/>
        </div>
    </div>    
</template>

<script>
import Project from './Project.vue'
export default {
    components: {
        Project
    },
    data() {
        return { 
            current: [
                { img:"pe1",  description: "Photo project management."},
                { img:"pe2",  description: "Photo Subjects."},
                { img:"pe3",  description: "Data import."},
            ],
            cap1: [
                { img:"cap1",  description: "Project management display board."},
                { img:"cap2",  description: "Weighted Shortest Job First (Agile development) analysis command board."},
            ],
            projects: [
                { img:"NYT", projectLink:"https://newyorktimesmernstack.herokuapp.com/", codeLink:"https://github.com/nosrednaski/nytReact", description: "Save your favorite NYT historical articles."},
                { img:"pouches2", projectLink:"http://pouches.herokuapp.com/", codeLink:"https://github.com/nosrednaski/Pouches", description: "Research your next KickStarter idea."},
                { img:"trivia2", projectLink:"https://nosrednaski.github.io/TriviaGame/", codeLink:"https://github.com/nosrednaski/TriviaGame", description: "Leaf Identification quiz"},
                { img:"gems", projectLink:"https://nosrednaski.github.io/gem-game/", codeLink:"https://github.com/nosrednaski/gem-game", description: "Math puzzle"},
            ],
        }
    },
    }
</script>

<style scoped lang="stylus">
    div.container 
        width 58%

        h1 
            text-align left
            font-size 2rem
            margin 1.5rem 0 

        div.grid
            display grid
            grid-template-columns: 1fr 1fr
            grid-column-gap: 3rem
            grid-row-gap: 4rem
            justify-items: center
            align-items: center
            margin-left: 2rem
            box-shadow: inset 1px 1px 2px rgba(0,0,0,.6);
            background-color rgba(0,0,0,.1)
            padding 1.6rem
            border-radius 7px
        
        div.four
            grid-template-rows: 1fr 1fr;

        
</style>
