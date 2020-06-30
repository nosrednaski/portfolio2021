<template>
  <div class="container1" data-aos="fade-down">
      <h1>Contact Me</h1>
      <div class="flex">
        <a href="mailto:nosrednaski@gmail.com?subject=Viewed%20your%20portfolio&body=Dearest%20nosrednaski%2C" target="_blank">
            <img src="../assets/mailto.svg" alt="mail to icon">
        </a>
        <a href="https://www.linkedin.com/in/jeffrey-anderson-731955141/" target="_blank" label="LinkedIn profile">
            <img src="../assets/linkedin.png" alt="linkedin icon">
        </a>
        
        
      </div>
  </div>    
</template>

<script>
export default {
  name: 'Contact',
  props: {
   
  }
}
</script>

<style scoped lang="stylus">
  div.container1
    
  div.textContainer 
    margin 4rem auto
    width 60%
    h1 
      text-align left
      font-size 2rem
      margin-bottom 2.4rem
  div.flex  
    display flex  
    a 
        margin-right 2rem
    a :hover   
      transform scale(1.1)   
    img
        height 4rem
        width 4rem
        

</style>
