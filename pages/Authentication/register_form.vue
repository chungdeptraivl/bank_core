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
      <register-form />
    </div>
  </div>
</template>

<script>
import registerForm from '~/components/auth/registerForm.vue'
export default {
  components: { registerForm },
  layout: 'authLayout'
}
</script>

<style></style>
 