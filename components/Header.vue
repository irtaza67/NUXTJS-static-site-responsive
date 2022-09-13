<!-- Please remove this file from your project -->
<template>
  <div>
    <div>
      <b-navbar toggleable="lg" type="dark">
        <b-navbar-brand href="#"><img src="/Logo.png" /></b-navbar-brand>
        <img class="px-2" src="seprator.svg" />
        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav>
            <b-nav-item-dropdown text="Quick Facts" right>
            </b-nav-item-dropdown>
            <b-nav-item-dropdown right>
              <!-- Using 'button-content' slot -->
              <template #button-content>
                <em>Benifits</em>
              </template>
            </b-nav-item-dropdown>
            <b-nav-item-dropdown right>
              <!-- Using 'button-content' slot -->
              <template #button-content>
                <em>Support</em>
              </template>
            </b-nav-item-dropdown>
          </b-navbar-nav>

          <!-- Right aligned nav items -->
          <b-navbar-nav class="ml-auto">
            <button class="get-in-touch">Get in Touch</button>
          </b-navbar-nav>
        </b-collapse>
      </b-navbar>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HeaderMain'
}
</script>
<style lang="scss">
.navbar-toggler {
  &.collapsed {
    background-color: black !important;
  }
  &.not-collapsed {
    background-color: black !important;
  }
}
.navbar-nav {
  a {
    color: #3d4d62 !important;
    font-size: 14px;
    padding-right: 28px !important;
    transition: 0.3s;
    &:first-child {
      padding-left: 15px !important;
    }
    &:hover {
      color: #01a4b7 !important;
    }
  }
  .dropdown-toggle::after {
    display: inline-block;
    background: url(/arrowdwn.svg) no-repeat !important;
    height: 7px;
    width: 10px;
    position: absolute;
    top: 15px;
    right: 10px;
    content: "";
    border-top: unset !important;
    border-right: unset !important;
    border-bottom: unset !important;
    border-left: unset !important;
  }
}
@media only screen and (max-width: 992px) {
    #nav-collapse{
    position: absolute;
    width: 100%;
    background: white;
    top: 100%;
    left: 0%;
    z-index: 1000;
  }
}
@media only screen and (max-width: 1024px) {
  .navbar-nav {
    text-align: center;
    button {
      display: none;
    }
    .dropdown-toggle::after {
      background: none !important;
    }
  }
}
</style>
