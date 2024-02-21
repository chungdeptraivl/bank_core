<template>
  <div class="wrapper">
    <div class="container">
      <div class="banner_content">
        <div class="picture_banner">
          <img class="banner-image" src="/images/card_jumbotron.jpeg" />
        </div>
        <div class="open_account">
          <h5>LIFE AND MONEY BY CITI</h5>
          <h1>
            Closing the Racial Wealth Gap
          </h1>
          <p>
            These are some keys to help create equitable pathways to income growth.
          </p>

          <b-button
            class="p-2"
            style="font-weight: bold; width: 200px; background: #056dae"
            >Learn more</b-button
          >
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.wrapper {
  width: 100vw;
  height: auto;
  background-color: #c5e4f3;
  padding: 40px 0;
}

.container {
  max-width: 90vw;
}

.banner_content {
  display: flex;
  align-items: center;
  justify-content: space-around;
  width: 100%;
}

.open_account {
  width: 30%;
  overflow: hidden;
  margin-top: 30px;
}

.picture_banner {
  overflow: hidden;
  height: 100%;
  border-radius: 16px;
}

.banner-image {
  width: 100%;
  height: 100%;
  object-fit: cover; /* Giữ tỷ lệ khung và điều chỉnh ảnh để lấp đầy khung */
}

.picture_banner img {
  display: none;
}

.picture_banner img:first-child {
  display: block;
}

/* Responsive CSS */
@media screen and (max-width: 1024px) {
  .banner_content {
    flex-direction: column-reverse; /* Chuyển layout thành dạng dọc và đảo ngược vị trí của hai phần tử con */
    text-align: center; /* Căn giữa nội dung */
  }

  .open_account {
    width: 100%; /* Phần mở tài khoản chiếm toàn bộ chiều rộng */
    margin-top: 0; /* Bỏ margin top */
    margin-bottom: 40px; /* Thêm margin bottom */
  }

  .picture_banner {
    width: 100%; /* Phần hình ảnh chiếm toàn bộ chiều rộng */
    padding: 20px 0;
  }
}
</style>
