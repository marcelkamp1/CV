<template>
  <div>
    <h2>
      <svg-icon type="mdi" class="mdi" :path="path" />
      Languages
    </h2>
    <table>
      <tr>
        <td class="attr">German</td>
        <td class="value">
          <AwesomeVueStarRating
            class="stars"
            :star="this.germanStar"
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
        <td class="attr">English</td>
        <td class="value">
          <AwesomeVueStarRating
            class="stars"
            :star="this.englishStar"
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
import { mdiTranslate } from '@mdi/js'

export default {
  name: 'Language',
  components: {
    AwesomeVueStarRating,
    SvgIcon
  },
  data () {
    return {
      path: mdiTranslate,
      germanStar: 5,
      englishStar: 4,
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
