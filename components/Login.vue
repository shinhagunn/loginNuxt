<template>
  <div class="login-block">
    <div class="login-main">
      <div class="login-another">
        <p class="register">
          Don't have an account yet? <a href="">Create one</a>
        </p>
      </div>

      <div class="login-form">
        <h2 class="title">Login to MyMusic</h2>
        <form action="">
          <div class="form-block">
            <label for="iemail">Email</label>
            <input
              class="form-control"
              id="iemail"
              type="email"
              name="email"
              placeholder="Email"
            />
          </div>
          <div class="form-block">
            <label for="ipassword">Password</label>
            <input
              class="form-control"
              id="ipassword"
              type="password"
              name="password"
              placeholder="Password"
            />
          </div>
          <div class="form-block">
            <input
              class="form-control btn"
              type="submit"
              name="submit"
              value="Sign In"
            />
          </div>
        </form>
        <a href="" class="forgot">Forgot Password?</a>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator'

@Component({})
export default class Login extends Vue {}
</script>

<style lang="less">
.login-block {
  position: absolute;
  right: 0;
  padding: 60px;
  width: 50%;
  height: 100%;
  background-color: #fff;

  a {
    text-decoration: none;
    color: rgb(119, 85, 229);
  }

  a:hover {
    text-decoration: underline;
  }

  .login-main {
    .login-another {
      .register {
        margin-bottom: 80px;
        text-align: right;
        font-size: 14px;
      }
    }

    .login-form {
      margin: 0 auto;
      width: 450px;

      .title {
        margin-bottom: 80px;
        display: inline-block;
        line-height: 36px;
        font-size: 24px;
        font-weight: 500;
        color: #6039de;
        border-bottom: solid 2px #6039de;
      }

      .form-block {
        margin: 18px 0;

        label {
          margin-bottom: 8px;
          display: inline-block;
          font-size: 16px;
        }

        .form-control {
          padding: 0 12px;
          width: 100%;
          height: 46px;
          display: block;
          background-color: #f5f7f9;
          border: 1px solid #fff;
          border-radius: 5px;
          transition: all 0.3s;
        }

        .form-control:hover {
          border: 1px solid #6039de;
        }

        .form-control:focus {
          border: 1px solid #6039de;
          outline: none;
        }

        .btn {
          margin-top: 120px;
          background-color: #7755e5;
          border: none;
          color: #fff;
          transition: all 0.3s;
        }

        .btn:hover {
          border: none;
          cursor: pointer;
          background-color: rgba(119, 85, 229, 0.85);
        }
      }

      .forgot {
        font-size: 14px;
      }
    }
  }
}
</style>