<template>
	<!-- Sidebar goes here  -->
	<div class="main">
		<div class="container">

		</div>
	</div>
	<AppFooter />
</template>

<script lang="ts">
import AppFooter from '@/components/app/Footer.vue'
export default {
	components: {
		AppFooter
	}
}
</script>

<style>
	html body {
		height: 100vh;
		margin: 0;
		font-family: arial, sans-serif;
	}

	#app {
		height: 100%
	}

	input:focus {
		outline: none;
	}

	.main {
		margin-left: 270px;
	}

	.container {
		display: flex;
		height: 100vh;
		width: 100%;
		justify-content: center;
		align-items: center;
		align-content: center;
	}
</style>