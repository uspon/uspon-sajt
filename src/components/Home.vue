<template>
	<div class="Home">
		<header class="masthead">
      <b-container class="intro-text">
        <b-row align-v="center" align-h="center" class="intro-text-container text-center">
          <b-col col>
            <p class="intro-lead-in">Udruženje slobodnog prosvećenog naroda.</p>
            <p class="intro-main">USPON</p>
          </b-col>
        </b-row>
      </b-container>
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
.masthead {
  height: calc(100vh - 106px);
}
.masthead .intro-text {
  height: 100%;
}
.masthead .intro-text .intro-text-container {
  height: 100%;
}
.intro-lead-in {
  font-size: 1.1em;
}
.intro-main {
  font-size: 6em;
}

@media screen and (max-width: 767px) {
  .Home {
    width: 100%;
    margin-left: 0;
  }
  /*.masthead .intro-text {
    margin-top: 50%;
  }*/
  .masthead .intro-text .intro-main {
    font-size: 4.5em;
  }
  .content {
    width: 95%;
    margin-left: calc((100% - 95%)/2);
  }
}
</style>
