<template>
  <header>
    <b-navbar toggleable="lg" type="dark" variant="dark">
      <b-navbar-brand href="/">
        Remoneer
      </b-navbar-brand>
      <b-collapse v-if="isRoot" id="nav-collapse" is-nav>
        <b-navbar-nav>
          <b-nav-item v-scroll-to="'#product'" href="/#product">
            Product
          </b-nav-item>
          <b-nav-item v-scroll-to="'#solution'" href="/#solution">
            Solution
          </b-nav-item>
          <b-nav-item v-scroll-to="'#team'" href="/#team">
            Team
          </b-nav-item>
          <b-nav-item href="/ask">
            Pricing
          </b-nav-item>
        </b-navbar-nav>
      </b-collapse>
      <b-collapse v-else id="nav-collapse" is-nav>
        <b-navbar-nav>
          <b-nav-item href="/#product">
            Product
          </b-nav-item>
          <b-nav-item href="/#solution">
            Solution
          </b-nav-item>
          <b-nav-item href="/#team">
            Team
          </b-nav-item>
          <b-nav-item href="/ask">
            Pricing
          </b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </header>
</template>

<script>
export default {
  data() {
    return { isRoot: this.$route.path === '/' }
  }
}
</script>

<style>
.navbar {
  padding-left: 80px;
  padding-right: 80px;
}

.nav-item {
  padding: 0 5px;
}

.navbar-collapse {
  padding-left: 20px;
}
</style>
