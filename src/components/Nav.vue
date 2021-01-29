
<template>
  <b-navbar fixed-top shadow data-aos="fade-up"  >

        <template slot="brand" >
            <b-navbar-item tag="div" class="name">
                <a href="https://drive.google.com/file/d/1AoFBDH56jbrT4horqV_gmz-Rf1kg0rfq/view?usp=sharing" data-content="Jeff Anderson" target="_blank">Jeff Anderson</a>
            </b-navbar-item>
        </template>
        

        <template slot="end">
            
            <b-navbar-item tag="a">
                <a href="https://github.com/nosrednaski" target="_blank">
                    <img src="../assets/github.svg" alt="github icon">
                </a>
            </b-navbar-item>
            <b-navbar-item tag="a" class="tail">
                <a href="https://drive.google.com/file/d/1AoFBDH56jbrT4horqV_gmz-Rf1kg0rfq/view?usp=sharing" target="_blank">
                    <img src="../assets/resume.png" alt="resume icon">
                </a>
            </b-navbar-item>
        </template>

    </b-navbar>
</template>

<script>

export default {
    components: {
    }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="stylus">
@import url('https://fonts.googleapis.com/css2?family=Merriweather:wght@900&display=swap');

$grey= rgba(0,0,0,.8)
div.navbar-item.name
    margin-left: 2rem
    a 
        position: relative
        display: inline-block
        font-size: 1.75em
        font-family: 'Merriweather', serif; 
        color: $grey
        font-weight: 500
        text-decoration: none
        overflow: hidden
        transition: clip-path 275ms ease
        &:hover::before 
          clip-path: polygon(0 0, 100% 0, 100% 100%, 0 100%)
        
        &::before 
          position: absolute
          content: attr(data-content)
          color: #006600
          text-decoration: underline
          clip-path: polygon(0 0, 0 0, 0% 100%, 0 100%)
          transition: clip-path 275ms ease
        

a.navbar-item 
    padding .4rem 0 0 0
    margin-left 1.3rem

    :hover
        transform scale(1.1)

a.navbar-item.tail
    margin-right: 3rem




</style>
