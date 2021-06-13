<template>
  <div id="app">
    <img src="@/assets/Profilbild.png" alt="Profilepicture" />
    <h1>Welcome to my CV!</h1>
    <p>
      On this page, you will find any necessary information about me, my
      degrees, as well as my working experience.
    </p>
    <p>
      If you have any further questions, please feel free to get in touch with
      me. You will find any relevant contact information below.
    </p>
    <compression />
  </div>
</template>

<script>
import Compression from '@/components/compression.vue'

export default {
  name: 'App',
  components: {
    Compression
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
</style>
