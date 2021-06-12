<template>
  <div>
    <h2>
      <svg-icon type="mdi" class="mdi" :path="path" />
      Programming Languages
    </h2>
    <table>
      <tr>
        <td><svg-icon type="mdi" class="mdi" :path="vuePath" /></td>
        <td class="value">
          <AwesomeVueStarRating
            class="stars"
            :star="this.vue"
            :disabled="this.disabled"
            :maxstars="this.maxstars"
            :starsize="this.starsize"
            :hasresults="this.hasresults"
            :hasdescription="this.hasdescription"
            :ratingdescription="this.ratingdescription"
          />
        </td>
      </tr>
      <tr>
        <td><svg-icon type="mdi" class="mdi" :path="javascriptPath" /></td>
        <td class="value">
          <AwesomeVueStarRating
            class="stars"
            :star="this.javascript"
            :disabled="this.disabled"
            :maxstars="this.maxstars"
            :starsize="this.starsize"
            :hasresults="this.hasresults"
            :hasdescription="this.hasdescription"
            :ratingdescription="this.ratingdescription"
          />
        </td>
      </tr>
      <tr>
        <td><svg-icon type="mdi" class="mdi" :path="htmlPath" /></td>
        <td class="value">
          <AwesomeVueStarRating
            class="stars"
            :star="this.html"
            :disabled="this.disabled"
            :maxstars="this.maxstars"
            :starsize="this.starsize"
            :hasresults="this.hasresults"
            :hasdescription="this.hasdescription"
            :ratingdescription="this.ratingdescription"
          />
        </td>
      </tr>
      <tr>
        <td><svg-icon type="mdi" class="mdi" :path="cssPath" /></td>
        <td class="value">
          <AwesomeVueStarRating
            class="stars"
            :star="this.css"
            :disabled="this.disabled"
            :maxstars="this.maxstars"
            :starsize="this.starsize"
            :hasresults="this.hasresults"
            :hasdescription="this.hasdescription"
            :ratingdescription="this.ratingdescription"
          />
        </td>
      </tr>
      <tr>
        <td><svg-icon type="mdi" class="mdi" :path="sassPath" /></td>
        <td class="value">
          <AwesomeVueStarRating
            class="stars"
            :star="this.sass"
            :disabled="this.disabled"
            :maxstars="this.maxstars"
            :starsize="this.starsize"
            :hasresults="this.hasresults"
            :hasdescription="this.hasdescription"
            :ratingdescription="this.ratingdescription"
          />
        </td>
      </tr>
      <tr>
        <td><svg-icon type="mdi" class="mdi" :path="javaPath" /></td>
        <td class="value">
          <AwesomeVueStarRating
            class="stars"
            :star="this.java"
            :disabled="this.disabled"
            :maxstars="this.maxstars"
            :starsize="this.starsize"
            :hasresults="this.hasresults"
            :hasdescription="this.hasdescription"
            :ratingdescription="this.ratingdescription"
          />
        </td>
      </tr>
    </table>
  </div>
</template>

<script>
import AwesomeVueStarRating from 'awesome-vue-star-rating'
import SvgIcon from '@jamescoyle/vue-icon'
import { mdiVuejs, mdiLaptop, mdiLanguageCss3, mdiLanguageHtml5, mdiLanguageJava, mdiLanguageJavascript, mdiSass } from '@mdi/js'

export default {
  name: 'ProgrammingLanguages',
  components: {
    AwesomeVueStarRating,
    SvgIcon
  },
  data () {
    return {
      path: mdiLaptop,
      vuePath: mdiVuejs,
      javascriptPath: mdiLanguageJavascript,
      cssPath: mdiLanguageCss3,
      sassPath: mdiSass,
      htmlPath: mdiLanguageHtml5,
      javaPath: mdiLanguageJava,
      vue: 4,
      javascript: 4,
      html: 4,
      css: 4,
      sass: 3,
      java: 3,
      ratingDescription: [
        {
          text: 'Poor',
          class: 'star-poor'
        },
        {
          text: 'Below Average',
          class: 'star-belowAverage'
        },
        {
          text: 'Average',
          class: 'star-average'
        },
        {
          text: 'Good',
          class: 'star-good'
        },
        {
          text: 'Excellent',
          class: 'star-excellent'
        }
      ],
      hasresults: false,
      hasdescription: true,
      starsize: 'lg',
      maxstars: 5,
      disabled: true
    }
  }
}
</script>

<style scoped>
h2 {
  text-align: center;
  margin: 40px 0 0;
  font-style: italic;
}
.attr {
  font-weight: bold;
}
.value {
  text-align: end;
}
.mdi {
  margin-right: 10px;
  width: 36px;
  height: 36px;
  transform: translateY(.5em);
}
table {
  margin: 0 !important;
}
table tr td {
  padding-top: 0 !important;
}
.stars {
  transform: translateY(-1.5em);
}
</style>
