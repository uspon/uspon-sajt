<template>
	<div class="Home">
		<header class="masthead">
      <b-container class="intro-text">
        <b-row align-v="center" align-h="center" class="intro-text-container text-center">
          <b-col col>
            <p class="intro-lead-in">Удружење слободног просвећеног народа.</p>
            <p class="intro-main">УСПОН</p>
          </b-col>
        </b-row>
      </b-container>
    </header>
    <section class="content">
      <section class="about">
        Удружење УСПОН је удружење које се бави уздизањем свести о културолошком наслеђу света,
        едукацијом првенствено младих, истраживачким радом и спортским активностима.
        Основали смо се са намером да људима пружимо нов и универзалан поглед на свет,
        поглед онога којег данас називамо ренесансним човеком. Трудимо се да успемо у својим
        нескромно речено племенитим циљевима како би активирали људе који су чак и заборавили
        колико је тако нешто важно.<br/><br/><br/>

        Срдачан поздрав,<br/>
        <span id="potpis">Лука З. Станковић</span>
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
@import url('https://fonts.googleapis.com/css?family=Bad+Script');

.Home {
  width: 1024px;
  margin-left: calc((100% - 1024px)/2);
}
.masthead {
  height: calc(100vh - 106px);
}
.masthead .intro-text {
  height: 100%;
  font-weight: 500;
}
.masthead .intro-text .intro-text-container {
  height: 100%;
}
.intro-lead-in {
  font-size: 1.5em;
  font-weight: 200;
}
.intro-main {
  font-size: 10em;
}
.about {
  font-size: 1.3em;
}
#potpis {
  font-family: 'Bad Script', cursive;
  font-size: 1.7em;
}

@media screen and (max-width: 1023px) {
  .Home {
    width: 768px;
    margin-left: calc((100% - 768px)/2);
  }
}

@media screen and (max-width: 767px) {
  .Home {
    width: 100%;
    margin-left: 0;
  }
  /*.masthead .intro-text {
    margin-top: 50%;
  }*/
  .intro-lead-in {
    font-size: 1.1em;
  }
  .masthead .intro-text .intro-main {
    font-size: 5em;
  }
  .content {
    width: 90%;
    margin-left: calc((100% - 90%)/2);
  }
  .about {
    font-size: 1em;
  }
}
</style>
