<template>
  <div
    class="container"
    style="
      border-radius: 8px;
      box-shadow: rgba(149, 157, 165, 0.2) 0px 8px 24px;
    "
  >
    <div class="signup-content">
      <div class="signup-image">
        <h2 class="form-title">Login Form</h2>

        <figure>
          <img
            src="/images/bank_login.avif"
            alt="sing up image"
            style="width: 100%; height: 100%; margin-top: 20px"
          />
          <a href="/Authentication/register_form" class="signup-image-link"
            >Create an account</a
          >
        </figure>
      </div>
      <div class="signup-form">
        <b-form>
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
              type="password"
              placeholder="Enter password"
              required
            ></b-form-input>
          </b-form-group>

          <b-form-group>
            <b-form-checkbox-group>
              <b-form-checkbox value="">Remember me</b-form-checkbox>
            </b-form-checkbox-group>
          </b-form-group>

          <b-form-group>
            <b-button type="submit" variant="primary">Login</b-button>
          </b-form-group>
        </b-form>
      </div>
    </div>
  </div>
</template>

<script>
export default {
}
</script>

<style scoped>
.container {
  padding: 50px;
}

.signup-content {
  display: flex;
  justify-content: center; /* Căn chỉnh các phần tử theo chiều ngang vào giữa */
  align-items: center; 
}

.signup-form {
  flex: 1; /* Sử dụng flex để phần form mở rộng khi không có ảnh */
  overflow: hidden;
  padding: 0 20px;
  margin-top: 70px;
}

.signup-image {
  flex: 1; /* Sử dụng flex để phần ảnh mở rộng khi không có form */
  margin-top: 45px;
  margin: 0 20px;
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
  margin-bottom: 20px;
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
