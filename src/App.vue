<template>
  <div id="app">
    <b-navbar toggleable="md" type="light" variant="faded" class="nav">
      <b-navbar-toggle target="nav_collapse" id="nav_bar_toggle"></b-navbar-toggle>
      <b-navbar-brand to="/" class="brand"><img src="./assets/uspon-logo-latin.png" alt="USPON" /></b-navbar-brand>
      <b-collapse is-nav id="nav_collapse" class="bold">
        <b-navbar-nav class="ml-auto">
          <b-nav-item to="/" exact>Почетна</b-nav-item>
          <b-nav-item-dropdown text="Тимови" id="timoviDropdown">
            <b-dropdown-item to="/team/knjizevni" exact class="dropdownItem">Књижевни</b-dropdown-item>
            <b-dropdown-item to="/team/muzicki" exact class="dropdownItem">Музички</b-dropdown-item>
            <b-dropdown-item to="/team/socioloski" exact class="dropdownItem">Социолошки</b-dropdown-item>
            <b-dropdown-item to="/team/likovni" exact class="dropdownItem">Ликовни</b-dropdown-item>
            <b-dropdown-item to="/team/dramski" exact class="dropdownItem">Драмски</b-dropdown-item>
            <b-dropdown-item to="/team/naucni" exact class="dropdownItem">Научни</b-dropdown-item>
            <b-dropdown-item to="/team/matematicki" exact class="dropdownItem">Математички</b-dropdown-item>
            <b-dropdown-item to="/team/istorijski" exact class="dropdownItem">Историјски</b-dropdown-item>
            <b-dropdown-item to="/team/sportski" exact class="dropdownItem">Спортски</b-dropdown-item>
            <b-dropdown-item to="/team/tehnoloski" exact class="dropdownItem">Технолошки</b-dropdown-item>
          </b-nav-item-dropdown>
          <b-nav-item to="/contact" exact>Контакт</b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
    <router-view/>
    <footer>
      <span>MIT License © USPON</span><br/>
      <span>Hosted on <a href="https://github.com">GitHub.com</a></span><br/>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Montserrat:200,300,400,500,600,700&subset=cyrillic-ext,latin-ext');

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  width: 100%;
  height: 100%;
  font-family: 'Montserrat', sans-serif;
}
.nav {
  border-radius: 5px;
  width: 1024px;
  margin-left: calc((100% - 1024px)/2);
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
.bold {
  font-weight: 600;
}

#timoviDropdown .dropdownItem {
  outline: none;
}
footer {
  margin-top: 50px;
  margin-bottom: 30px;
  text-align: center;
}

@media screen and (max-width: 1023px) {
  .nav {
    width: 768px;
    margin-left: calc((100% - 768px)/2);
  }
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
