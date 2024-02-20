<template>
  <b-navbar
    toggleable="lg"
    type="light"
    class="p-3"
    style="box-shadow: rgba(99, 99, 99, 0.2) 0px 2px 8px 0px"
  >
    <b-navbar-brand href="/"> CT CREDIT </b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item class="nav_item" href="#">Credit Cards</b-nav-item>
        <b-nav-item class="nav_item" href="#">Banking</b-nav-item>
        <b-nav-item class="nav_item" href="#">Lending</b-nav-item>
        <b-nav-item class="nav_item" href="#">Investing</b-nav-item>
        <b-nav-item class="nav_item" href="#">Wealth Management</b-nav-item>
      </b-navbar-nav>

      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <b-nav-item-dropdown text="Lang" right>
          <b-dropdown-item href="#">EN</b-dropdown-item>
          <b-dropdown-item href="#">ES</b-dropdown-item>
          <b-dropdown-item href="#">RU</b-dropdown-item>
          <b-dropdown-item href="#">FA</b-dropdown-item>
        </b-nav-item-dropdown>

        <b-nav-item-dropdown right>
          <!-- Using 'button-content' slot -->
          <template #button-content>
            <em>User</em>
          </template>
          <b-dropdown-item href="#">Profile</b-dropdown-item>
          <b-dropdown-item href="#">Sign Out</b-dropdown-item>
        </b-nav-item-dropdown>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</template>

<script>
export default {}
</script>

<style scoped>
.nav_item {
    font-weight: bold;
    margin-left: 16px;
}

.nav_item:hover {
    color: #f0f5f7;
}
</style>
