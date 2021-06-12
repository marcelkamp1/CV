<template>
  <div id="app">
    <img src="@/assets/Profilbild.png" alt="Profilepicture">
    <h1>Welcome to my CV!</h1>
    <p>
      On this page, you will find any necessary information about me,
      my degrees, as well as my working experience.
    </p>
    <p>
      If you have any further questions, please feel free to get in touch with me.
      You will find any relevant contact information below.
    </p>
    <personal-info class="personalInfo right-sided" />
    <skills class="skills right-sided" />
    <language class="language right-sided" />
    <programming-languages class="programming right-sided" />
  </div>
</template>

<script>
import PersonalInfo from '@/components/right-sided/personalInfo'
import Skills from '@/components/right-sided/skills'
import Language from '@/components/right-sided/language.vue'
import ProgrammingLanguages from '@/components/right-sided/programmingLanguages.vue'

export default {
  name: 'App',
  components: {
    PersonalInfo,
    Skills,
    Language,
    ProgrammingLanguages
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
  margin-left: 1.5em;
}
img {
  width: 256px;
  height: 256px;
}
table {
  width: 340px;
  margin: 10px auto;
  text-align: start;
}
table tr td {
  padding: 5px 20px;
}
.right-sided {
  position: absolute;
  right: 1.5em;
  padding: 1em 1em 2.5em;
}
.personalInfo {
  top: -3em;
}
.skills {
  top: 20em;
}
.language {
  top: 47em;
}
.programming {
  top: 72em;
}
</style>
