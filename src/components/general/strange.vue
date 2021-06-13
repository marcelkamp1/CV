<template>
  <div class="footer">
    <a href="https://www.github.com">
      <svg-icon type="mdi" :path="mdiGithub" />
    </a>
  </div>
</template>

<script>
import SvgIcon from '@jamescoyle/vue-icon'
import { mdiGithub } from '@mdi/js'

export default {
  name: 'strange',
  components: {
    SvgIcon
  },
  data () {
    return {
      path: mdiGithub
    }
  }
}
</script>

<style scoped>
.footer {
  border: 1px solid #000;
  height: 50px;
}
</style>
