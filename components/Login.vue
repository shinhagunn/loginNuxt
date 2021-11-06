<template>
  <div class="login">
    <div class="logo">
      <h1 class="logo-name">My music</h1>
    </div>

    <form action="" class="form">
      <div class="form-block">
        <input
          class="form-control"
          type="email"
          name="email"
          placeholder="Email"
        />
      </div>

      <div class="form-block">
        <input
          class="form-control"
          type="password"
          name="password"
          placeholder="Password"
        />
      </div>

      <div class="form-block">
        <input
          class="form-control bton"
          type="submit"
          name="sub"
          value="Login"
        />
      </div>
    </form>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator'

@Component({})
export default class Login extends Vue {
  ten = 'hoang'
}
</script>

<style lang="less">
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: Arial, Helvetica, sans-serif;
}

.login{
    margin: 50px auto;
    width: 350px;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.logo{
    .logo-name{
        padding: 20px;
        font-size: 40px;
    }
}

.form{
    .form-control{
        margin-bottom: 20px;
        padding: 0 20px;
        width: 350px;
        height: 50px;
        border: 1px solid #000;
    }

    .form-control:hover{
        border-color: #29adff;
    }

    .form-control:focus{
        outline: none;
        border-color: #29adff;
    }

    .bton{
        background-color: #29adff;
        color: #fff;
        font-size: 18px;
        border-color: #29adff;
    }

    .bton:hover{
        cursor: pointer;
    }
}
</style>