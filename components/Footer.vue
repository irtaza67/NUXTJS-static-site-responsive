<!-- Please remove this file from your project -->
<template>
  <div class="relative d-flex footer pt-3">
    <ul class="d-flex f-16">
      <li><NuxtLink to="/">Imprint</NuxtLink></li>
      <li><NuxtLink to="/">Data Security</NuxtLink></li>
      <li><NuxtLink to="/">Conditions</NuxtLink></li>
      <li><NuxtLink to="/">Cookies</NuxtLink></li>
      <li><NuxtLink to="/">Custom support</NuxtLink></li>
    </ul>
    <div class="copy-rights">
      <p class="f-14">© 2021 Customs Support Group. All rights reserved.</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'FooterMain'
}
</script>
<style lang="scss" scoped>
.footer {
  justify-content: space-around;
}
ul {
  list-style: none;
  a {
    color: #3d4d62;
    padding: 0px 8px;
  }
}
@media only screen and (max-width: 1024px) {
  .footer {
    display: block !important;
    li {
      margin: 8px 0px;
    }
  }
}
</style>
