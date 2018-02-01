<template>
	<div class="Contact">
		<header>
			<h1>Kontakt</h1>
		</header>
		<section>
			<br/>
			<p>Ukoliko želite da nas kontaktirate ovde možete naći potrebne informacije.</p>
			<br/>
			<div class="osoba">
				<h3>Neko Ime</h3>
				<img src="../assets/uspon-logo-latin.png" alt="Neka slika"/>
				<ul>
					<li>Br. tel. : <strong>brojfona</strong></li>
					<li>E-Mail: <strong><a href="mailto:mejl">mejl</a></strong></li>
				</ul>
			</div>
		</section>
	</div>
</template>

<script>
export default {
	name: 'Contact'
}
</script>

<style>
.Contact {
	width: 700px;
	margin-left: calc((100% - 700px)/2);
	margin-top: 10%;
}
.osoba img {
	width: 200px;
	height: auto;
}

@media screen and (max-width: 767px) {
	.Contact {
		width: 95%;
		margin-left: calc((100% - 95%)/2);
		margin-top: 10%;
	}
	.osoba img {
		width: 60%;
	}
}
</style>
