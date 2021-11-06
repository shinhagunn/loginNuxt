<template>
  <div class="loginPage">
    <Login/>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator'

@Component({})
export default class loginPage extends Vue {
  
}
</script>

<style lang="less">
*{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
html{
  background: url('../content/img/background_login.jpg') no-repeat;
  background-size: cover;
  font-family: Arial, Helvetica, sans-serif;
}
</style>
