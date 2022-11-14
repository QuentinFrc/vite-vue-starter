<script setup>

defineProps({
	title: String
})

</script>

<template>
	<header>
		<div class="header-part header-left">
			<h1>{{ title }}</h1>
		</div>
		<div class="header-part header-right">

		</div>
	</header>
</template>

<style lang="scss" scoped>

@use "src/scss/variables" as vr;

header {
	min-height: 100vh;
	display: flex;
	align-items: stretch;

	.header-part{
		flex: 1;
	}

	.header-left{
		display: flex;
		flex-direction: column;
		gap: vr.$space-1;
	}
}
</style>
