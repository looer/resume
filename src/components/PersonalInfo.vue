<template lang="pug">
    .rightBox#PersonalInfo
        h1 {{name}}
        p 🏠 {{address}}
        p 📱 {{phone}}
        p 📧 {{email}}
</template>

<script>
export default {
    name: "PersonalInfo",
    props: {
        name: String,
        address: String,
        phone: String,
        email: String
    }
}
</script>

<style lang="stylus" scoped>
h1
    margin: 0px
    padding: 0px

.rightBox
    margin: 0px 30px

</style>
