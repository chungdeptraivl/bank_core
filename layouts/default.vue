<template>
  <div>
    <header-layout />
    <nuxt />
    <footer-layout />
  </div>
</template>

<script>
import FooterLayout from '~/components/layout/footerLayout.vue'
import headerLayout from '~/components/layout/headerLayout.vue'
export default {
  components: { headerLayout, FooterLayout },
}
</script>

<style></style>
