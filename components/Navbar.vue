<template>
  <div class="page">
    <b-navbar
      fluid
      class="nav"
      toggleable="lg"
    >
      <b-navbar-brand href="/">AnansiWeb8.zil</b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse
        id="nav-collapse"
        is-nav
      >
        <b-navbar-nav>
          <b-nav-item href="/blocksites">Blocksites</b-nav-item>
          <b-nav-item href="/decentralized">Decentraland</b-nav-item>
        </b-navbar-nav>

        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-nav-form>
            <b-form-input
              size="sm"
              class="mr-sm-2"
              placeholder="Search"
            ></b-form-input>
            <b-button
              size="sm"
              class="my-2 my-sm-0"
              type="submit"
              id="go"
            >Search</b-button>
          </b-nav-form>

          <b-nav-item-dropdown
            class="drop"
            text="More"
            right
          >
            <b-dropdown-item href="/Aboutanansi">About</b-dropdown-item>
            <b-dropdown-item href="/ads">Advertise</b-dropdown-item>
            <b-dropdown-item href="/domainwall">DomainWall</b-dropdown-item>
            <b-dropdown-item href="/Domainvision">DomainVision</b-dropdown-item>
            <b-dropdown-item href="/Non-custodialwallet">
              Non-custodial Wallets</b-dropdown-item>
            <b-dropdown-item href="/tutorial"> Tutorial</b-dropdown-item>
          </b-nav-item-dropdown>
          <b-nav-item> v{{ v }} </b-nav-item>

          <!-- Using 'button-content' slot -->
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data () {
    return {
      v: "0.0.01"
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.navbar .navbar-dark .bg-dark .navbar-expand-lg {
  border-bottom: 10px;
}

h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

.nav {
  background-color: #42b983;
  position: static;
}
.drop {
  background-color: #344a5f;
}
</style>
