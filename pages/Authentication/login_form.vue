<template>
  <div
    class="container"
    style="
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      transition: opacity 0.3s ease-in-out;
    "
  >
    <div class="p-4">
      <login-form />
    </div>
  </div>
</template>

<script>
import LoginForm from '~/components/auth/loginForm.vue'
export default {
  components: { LoginForm },
  layout: 'authLayout',
}
</script>

<style></style>
