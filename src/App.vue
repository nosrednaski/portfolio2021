<template>
  <div id="app">
    <Nav/>
    <Parallax/>
    <ProjectsContainer/>
    <About/>
    <Contact/>
    <Parallax/>

  </div>
</template>

<script>
import About from './components/About.vue';
import Nav from './components/Nav.vue';
import Parallax from './components/Parallax.vue';
import ProjectsContainer from './components/ProjectsContainer.vue';
import Contact from './components/Contact.vue';

export default {
  name: 'App',
  components: {
    About,
    Nav,
    Parallax,
    ProjectsContainer,
    Contact
  }
}
</script>

<style lang="stylus">
$grey= rgba(0,0,0,.7)
#app 
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  background #F6F4F3
  color $grey

  


/* 040F0F
4E937A
EFF9F0
F87060
5688C7 */
</style>
