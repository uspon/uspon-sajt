<template>
  <div id="app">
    <b-navbar toggleable="md" type="light" variant="faded" class="nav">
      <b-navbar-toggle target="nav_collapse" id="nav_bar_toggle"></b-navbar-toggle>
      <b-navbar-brand to="/" class="brand"><img src="./assets/uspon-logo-latin.png" alt="USPON" /></b-navbar-brand>
      <b-collapse is-nav id="nav_collapse">
        <b-navbar-nav class="ml-auto">
          <b-nav-item to="/" exact>Početna</b-nav-item>
          <b-nav-item to="/contact" exact>Kontakt</b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
    <router-view/>
    <footer>
      <span>MIT License © USPON</span><br/>
      <span>Hosted on <a href="https://github.com/uspon/uspon.github.io">GitHub.com</a></span><br/>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  width: 100%;
  height: 100%;
}
.nav {
  border-radius: 5px;
  margin-top: 10px;
  width: 700px;
  margin-left: calc((100% - 700px)/2);
  background-color: white;
}
.nav #nav_bar_toggle {
  outline: none;
}
.nav .brand {
  margin-right: calc((100% - 70px)/2) !important;
}
.nav .brand img {
  width: 70px;
  height: 70px;
}
footer {
  margin-top: 50px;
  text-align: center;
}

@media screen and (max-width: 767px) {
  .nav {
    border-radius: 0;
    margin-top: 0;
    width: 100%;
    margin-left: 0;
  }
  .nav #nav_collapse {
    font-size: 1.1em;
    text-align: center;
  }
  footer {
    margin-top: 15%;
  }
}
</style>
