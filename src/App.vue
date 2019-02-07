<template lang="pug">
  div(id="app")
    .top
      #profile
        img(alt="profile pic" src="./assets/profile.jpg")
      PersonalInfo( name="Lorenzo Cella"
                  address="Heugatterstrasse 22,\n8600 Dubendorf"
                  phone="+41 76 2211 033"
                  email="lorenz.cella@gmail.com")
    Experience( company="Autoneum Management AG" 
                position="Software Engineer" 
                description="Maintain an old codebase, optimizing the code and developing new features" 
                field="Software Development"
                date="November 2018 - April 2019")
    Experience( company="Bolt Motion SRL" 
                position="Founder & CEO" 
                description="Managing and taking care of everything" 
                field="Entrepreneurship"
                date="2015 - Today")           
</template>

<script>
import Experience from "./components/Experience.vue";
import PersonalInfo from "./components/PersonalInfo.vue";

export default {
  name: "app",
  components: {
    Experience,
    PersonalInfo
  }
};
</script>

<style lang="stylus">
#app
  font-family: "Avenir", Helvetica, Arial, sans-serif
  -webkit-font-smoothing: antialiased
  -moz-osx-font-smoothing: grayscale
  text-align: left
  color: #2c3e50
  margin: 60px 60px 10px 10px

.top
  display: flex

#profile
  flex: 0 0 25%

img
  width: 200px
  height: auto
  border-radius: 100%
  margin: 0 0 0 30px

PersonalInfo 
  flex: 1

</style>
