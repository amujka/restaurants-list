<template>
  <div>
    <slot name="errorTitle" />
    <div>
      <img
        src="https://e7.pngegg.com/pngimages/570/612/png-clipart-bankier-pl-http-404-web-page-bank-bank-%D0%BD%D0%B5-%D0%BD%D0%B0%D0%B9%D0%B4%D0%B5%D0%BD%D0%BE.png"
        alt="404"
      />
    </div>
    <slot name="redirectLink" />
  </div>
</template>

<script setup lang="ts"></script>

<style scoped lang="scss">
img {
  width: 100%;
}
</style>
