<template>
  <div
    class="container"
    style="
      border-radius: 8px;
      box-shadow: rgba(149, 157, 165, 0.2) 0px 8px 24px;
    "
  >
    <div class="signup-content">
      <div class="signup-form">
        <h2 class="form-title">Register Form</h2>
        <b-form>
          <b-form-group label="Username:" label-for="username">
            <b-form-input
              id="username"
              type="text"
              placeholder="Enter username"
              required
            ></b-form-input>
          </b-form-group>

          <b-form-group label="Email address" label-for="email">
            <b-form-input
              id="email"
              type="email"
              placeholder="Enter email address"
              required
            ></b-form-input>
          </b-form-group>

          <b-form-group label="Password" label-for="password">
            <b-form-input
              id="password"
              :type="passwordType"
              placeholder="Enter password"
              required
            ></b-form-input>
          </b-form-group>

          <b-form-group>
            <b-form-checkbox v-model="showPassword">
              Show password
            </b-form-checkbox>
          </b-form-group>

          <b-form-group>
            <b-button type="submit" variant="primary">Register</b-button>
          </b-form-group>
        </b-form>
      </div>
      <div class="signup-image">
        <figure>
          <img
            src="/images/bank_register.png"
            alt="sing up image"
            style="width: 100%; height: 100%; margin-top: 50px"
          />
          <a href="/Authentication/login_form" class="signup-image-link"
            >I am already member</a
          >
        </figure>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      showPassword: false,
    }
  },

  computed: {
    passwordType() {
      return this.showPassword ? 'text' : 'password'
    },
  },
}
</script>

<style scoped>
.container {
  padding: 50px;
}

.signup-content {
  display: flex;
  justify-content: center; /* Căn chỉnh các phần tử theo chiều ngang vào giữa */
  align-items: center; /* Thêm flex-wrap để các phần tử chuyển dòng khi không đủ không gian */
}

.signup-form {
  flex: 1; /* Sử dụng flex để phần form mở rộng khi không có ảnh */
  padding-left: 34px;
  overflow: hidden;
}

.signup-image {
  flex: 1; /* Sử dụng flex để phần ảnh mở rộng khi không có form */
  margin-top: 30px;
}

.form-title {
  margin-bottom: 33px;
  margin-bottom: 20px;
}

h2 {
  line-height: 1.66;
  margin: 0;
  padding: 0;
  font-weight: bold;
  color: #222;
  font-family: Arial, Helvetica, sans-serif;
  font-size: 36px;
}

figure {
  margin-bottom: 50px;
  text-align: center;
}

.signup-image-link {
  font-size: 16px;
  color: #222;
  text-align: center;
}

/* Điều chỉnh layout khi màn hình nhỏ hơn 1024px */
@media screen and (max-width: 1024px) {
  .signup-content {
    flex-direction: column; /* Chuyển sang layout dọc */
  }
  .signup-form,
  .signup-image {
    width: 100%; /* Phần tử chiếm toàn bộ chiều rộng */
  }
}
</style>
