<template>
	<div class="Tim">
		<header>
			<h1>Неки тим</h1>
		</header>
	</div>
</template>

<script>
export default {
	name: 'Tim',
	data () {
		return {
			teamName: this.$route.params.name
		}
	},
	watch: {
		'$route' (to, from) {
			this.teamName = this.$route.params.name
		}
	},
	methods: {
		fetchTexts () {
			
		}
	}
}
</script>

<style>

</style>
