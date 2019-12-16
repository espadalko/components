<template>
	<div class="menu">
		<div class="menu__item">Item1</div>
		<div class="menu__item">Item2</div>
		<div class="menu__item">Item3</div>
		<div class="menu__item">Item4</div>
		<div class="menu__item">Item5</div>
	</div>
</template>

<script>
	export default {
		name: 'MenuFix'
	}
	
</script>

<style lang="stylus">
	.menu
		display flex
		justify-content space-around
		flex-wrap wrap
		&__item
			&:hover
				cursor pointer
</style>