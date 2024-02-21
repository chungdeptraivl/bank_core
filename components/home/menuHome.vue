<template>
  <div class="wrapper container">
    <b-row class="list-items container d-flex align-center">
      <b-col class="item col='2' m-2">
        <i class="icon-item">
          <font-awesome-icon class="icon" :icon="['fas', 'credit-card']" />
        </i>
        <h6 class="name-item">Credit cards</h6>
      </b-col>
      <b-col class="item col='2' m-2">
        <i class="icon-item">
          <font-awesome-icon class="icon" :icon="['fas', 'house']" />
        </i>
        <h6 class="name-item">Mortgage</h6>
      </b-col>
      <b-col class="item col='2' m-2">
        <i class="icon-item">
          <font-awesome-icon :icon="['fas', 'shield-halved']" />
        </i>
        <h6 class="name-item">Checking solution</h6>
      </b-col>
      <b-col class="item col='2' m-2">
        <i class="icon-item">
          <font-awesome-icon :icon="['fas', 'money-bill-1-wave']" />
        </i>
        <h6 class="name-item">Money loans</h6>
      </b-col>
      <b-col class="item col='2' m-2">
        <i class="icon-item">
          <font-awesome-icon :icon="['fas', 'sliders']" />
        </i>
        <h6 class="name-item">Investing option</h6>
      </b-col>
      <b-col class="item col='2' m-2">
        <i class="icon-item">
          <font-awesome-icon :icon="['fas', 'tag']" />
        </i>
        <h6 class="name-item">Small business</h6>
      </b-col>
    </b-row>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.wrapper {
  border: #065180 1px solid;
  border-radius: 12px;
  background-color: #f6f6f6;
  max-width: 76vw;
}

.list-items {
  width: 100%;
  margin-top: 20px;
  justify-content: space-around;
  list-style: none;
  max-width: 100vw;
}

.item {
  display: flex;
  align-items: center;
  flex-direction: column;
}

.icon-item {
  width: 45px;
  height: 45px;
  border-radius: 50%;
  background: #eff3f8;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 18px;
}

.name-item {
  margin-top: 8px;
  text-align: center;
}

.item:hover {
  cursor: pointer;
}

.item:hover .icon-item {
  background-color: #066dae; /* Màu nền của icon-item khi hover */
  color: #eff3f8;
  cursor: pointer;
}

.item:hover .name-item {
  color: #066dae; /* Màu chữ của name-item khi hover */
  cursor: pointer;
}
</style>
