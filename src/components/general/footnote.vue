<template>
  <div class="footer">
    <a href="mailto:marcelkamp1@gmx.de">
      <svg-icon type="mdi" class="mdi mail" :path="pathMail" />
    </a>
    <a href="https://github.com/marcelkamp1" target="_blank" rel="noopener">
      <svg-icon type="mdi" class="mdi github" :path="pathGithub" />
    </a>
    <a href="https://www.linkedin.com" target="_blank" rel="noopener">
      <svg-icon type="mdi" class="mdi linkedin" :path="pathLinkedin" />
    </a>
    <a href="https://twitter.com/Harribo65" target="_blank" rel="noopener">
      <svg-icon type="mdi" class="mdi twitter" :path="pathTwitter" />
    </a>
    <a href="https://www.xing.com/profile/Marcel_Kamp7/cv" target="_blank" rel="noopener">
      <svg-icon type="mdi" class="mdi xing" :path="pathXing" />
    </a>
    <p>
      <strong>© by Marcel Kamp, 2021</strong>
    </p>
  </div>
</template>

<script>
import SvgIcon from '@jamescoyle/vue-icon'
import { mdiEmail, mdiGithub, mdiLinkedin, mdiTwitter, mdiXing } from '@mdi/js'

export default {
  name: 'Footnote',
  components: {
    SvgIcon
  },
  data () {
    return {
      pathMail: mdiEmail,
      pathGithub: mdiGithub,
      pathLinkedin: mdiLinkedin,
      pathTwitter: mdiTwitter,
      pathXing: mdiXing
    }
  }
}
</script>

<style scoped>
.footer {
  position: fixed;
  margin-left: -1.5em;
  width: 100%;
  bottom: 0;
  height: 75px;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  background-color: #c9feff;
}
.mdi {
  width: 36px;
  height: 36px;
}
.github {
  color: #000;
}
.twitter {
  color: #1DA1F2;
}
.linkedin {
  color: #0e76a8;
}
.xing {
  color: #126567;
}
</style>
