<template>
  <div>
    <personal-info class="personalInfo right-sided" />
    <skills class="skills right-sided" />
    <language class="language right-sided" />
    <programming-languages class="programming right-sided" />
    <footnote />
  </div>
</template>

<script>
import PersonalInfo from '@/components/right-sided/personalInfo'
import Skills from '@/components/right-sided/skills'
import Language from '@/components/right-sided/language'
import ProgrammingLanguages from '@/components/right-sided/programmingLanguages'
import Footnote from '@/components/general/footnote'

export default {
  name: 'Compression',
  components: {
    PersonalInfo,
    Skills,
    Language,
    ProgrammingLanguages,
    Footnote
  }
}
</script>

<style>
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
  padding-bottom: 6em;
}
</style>
