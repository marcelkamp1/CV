<template>
  <div>
    <h2>
      <svg-icon type="mdi" class="mdi" :path="path" />
      Skills
    </h2>
    <table>
      <tr>
        <td class="attr">Agile Frontend Developer</td>
      </tr>
      <tr>
        <td class="attr">Budget Management</td>
      </tr>
      <tr>
        <td class="value">planning of costs for internal and external employees as team manager</td>
      </tr>
      <tr>
        <td class="attr">Releasemanagement</td>
      </tr>
      <tr>
        <td class="value">planning + monitoring of regular releases</td>
      </tr>
      <tr>
        <td class="attr">Java development incl. Spring Framework</td>
      </tr>
      <tr>
        <td class="attr">App development in Java</td>
      </tr>
    </table>
  </div>
</template>

<script>
import SvgIcon from '@jamescoyle/vue-icon'
import { mdiPuzzle } from '@mdi/js'

export default {
  name: 'Skills',
  components: {
    SvgIcon
  },
  data () {
    return {
      path: mdiPuzzle
    }
  }
}
</script>

<style scoped>
h2 {
  text-align: center;
  margin: 40px 0 20px;
  font-style: italic;
}
.attr {
  font-weight: bold;
}
.value {
  font-style: italic;
}
.mdi {
  margin-right: 10px;
  width: 36px;
  height: 36px;
  transform: translateY(.3em);
}
</style>
