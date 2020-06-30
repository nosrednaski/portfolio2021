<template>
  <div class="container">
      <h1>Projects</h1>
        <div class="grid">
            <Project v-for="project in projects" :img="project.img" :projectLink="project.projectLink" :codeLink="project.codeLink" :description="project.description" :key="project.img"/>
        </div>
  </div>    
</template>

<script>
import Project from './Project.vue'
export default {
  name: 'ProjectsContainer',
  components: {
      Project
  },
  data() {
      return { 
          projects: [
          { img:"NYT", projectLink:"https://newyorktimesmernstack.herokuapp.com/", codeLink:"https://github.com/nosrednaski/nytReact", description: "Save your favorite NYT historical articles."},
          { img:"pouches2", projectLink:"http://pouches.herokuapp.com/", codeLink:"https://github.com/nosrednaski/Pouches", description: "Research your next KickStarter idea."},
          { img:"trivia2", projectLink:"https://nosrednaski.github.io/TriviaGame/", codeLink:"https://github.com/nosrednaski/TriviaGame", description: "Leaf Identification quiz"},
          { img:"gems2", projectLink:"https://nosrednaski.github.io/gem-game/", codeLink:"https://github.com/nosrednaski/gem-game", description: "Math puzzle"},
        ],
       }
  },
}
</script>

<style scoped lang="stylus">
  .container 
    width 60%
  h1 
      text-align left
      font-size 2rem
      margin 1.5rem 0 1.5rem 0 
      
    div.grid 
        display grid
        grid-template-columns: 1fr 1fr
        grid-template-rows: 1fr 1fr;
        grid-column-gap: 3rem
        grid-row-gap: 4rem
        justify-items: center
        align-items: center
</style>
