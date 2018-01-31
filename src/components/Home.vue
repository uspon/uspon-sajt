<template>
	<div class="Home">
		<header class="masthead">
      <b-navbar toggleable="md" type="light" variant="light" class="nav">
        <b-navbar-brand to="/" class="brand">USPON</b-navbar-brand>
        <b-collapse is-nav id="nav_collapse">
          <b-navbar-nav>
            <b-nav-item to="/contact">Contact</b-nav-item>
          </b-navbar-nav>
        </b-collapse>
        <b-navbar-toggle target="nav_collapse"></b-navbar-toggle>
      </b-navbar>
      <div class="logo"></div>
    </header>
    <section class="content">
      <section class="about">
        some text
      </section>
    </section>
	</div>
</template>

<script>
export default {
  name: "Home"
};
</script>

<style>
.masthead {
  width: 700px;
  height: 100vh;
  margin-left: calc((100% - 700px)/2);
}
.masthead .nav {
  border-radius: 5px;
  margin-top: 10px;
}
.masthead .nav .brand {
  display: none;
}
.masthead .logo {
  width: 100%;
  height: 100%;
  margin-left: 0;
  background-image: url('../assets/uspon-logo-latin.jpg');
  background-repeat: no-repeat;
  background-position: center;
  background-size: 60%;
}

@media screen and (max-width: 767px) {
	.masthead {
    width: 100%;
    height: 80vh;
    margin-left: 0;
    margin-bottom: 10vh;
	}
  .masthead .nav {
    border-radius: 0;
    margin-top: 0;
  }
  .masthead .nav .brand {
    display: inline;
  }
  .masthead .nav #nav_collapse {
    font-size: 1.1em;
    text-align: center;
  }
  .masthead .logo {
    width: 100%;
    height: 100%;
  }
}
</style>
