<template>
	<div class="Home">
		<header class="masthead">
      <div class="intro-text">
        <div class="intro-lead-in">Udruženje slobodnog prosvećenog naroda.</div>
        <div class="intro-main">USPON</div>
      </div>
    </header>
    <section class="content">
      <section class="about">
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
.Home {
  width: 700px;
  margin-left: calc((100% - 700px)/2);
}
.masthead .intro-text {
  margin-top: calc((50% - 106px)/2);
  margin-bottom: 50%;
  text-align: center;
}
.masthead .intro-text .intro-lead-in {
  font-size: 1.1em;
}
.masthead .intro-text .intro-main {
  font-size: 6em;
}

@media screen and (max-width: 767px) {
  .Home {
    width: 100%;
    margin-left: 0;
  }
  .masthead .intro-text {
    margin-top: 50%;
  }
  .masthead .intro-text .intro-main {
    font-size: 4.5em;
  }
  .content {
    width: 95%;
    margin-left: calc((100% - 95%)/2);
  }
}
</style>
