<template>
  <div class="wrapper">
    <div class="container">
      <div class="banner_content">
        <div class="open_account">
          <h5>CT CREDIT CHECHING ACCOUNTS</h5>
          <h1>
            Open. Deposit. <br />
            Earn $300.
          </h1>
          <p>
            Earn a bonus when you open an eligible checking account with
            Enhanced Direct Deposits & required activities.
          </p>

          <b-button
            class="p-2"
            style="font-weight: bold; width: 200px; background: #056dae"
            >Learn more</b-button
          >
        </div>

        <div class="picture_banner">
          <img src="/images/banking_app.png" alt="">
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
  height: 40vh;
  background-image: url('/images/bgr_banner.jpeg');
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
}

.picture_banner > img {
  height: 40vh;
}
</style>
