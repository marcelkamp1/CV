<template>
  <div>
    <h2>
      <md-avatar class="md-avatar-icon">
        <img src="@/assets/Profilbild.png" alt="profile">
      </md-avatar>
      Personal Details
    </h2>
    <table>
      <tr>
        <td class="attr">Salutation:</td>
        <td class="value">Herr / Mr.</td>
      </tr>
      <tr>
        <td class="attr">Name:</td>
        <td class="value">Marcel Kamp</td>
      </tr>
      <tr>
        <td class="attr">Date of Birth:</td>
        <td class="value">10. June 1992</td>
      </tr>
      <tr>
        <td class="attr">Street:</td>
        <td class="value">Mozartstraße 9</td>
      </tr>
      <tr>
        <td class="attr">Zip Code:</td>
        <td class="value">53773</td>
      </tr>
      <tr>
        <td class="attr">City:</td>
        <td class="value">Hennef</td>
      </tr>
    </table>
  </div>
</template>

<script>
export default {
  name: 'PersonalInfo'
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
.md-avatar-icon {
  margin-right: 10px;
}
</style>
