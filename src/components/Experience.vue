<template lang="pug">
  .Experience
    h2 {{position}}
    h4 {{company}}
    p {{description}}
    small {{field}}
    small {{date}}
    hr
</template>


<script>
export default {
  name: "Experience",
  props: {
    company: String,
    position: String,
    description: String,
    field: String,
    date: String
  }
};
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="stylus" scoped>
.Experience
  margin: 50px
  align: right

hr
  margin: 30px 0

h3
  margin: 40px 0 0

a {
  color: #42b983;
}
</style>
