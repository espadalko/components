<template>
	<div id="app">
		<div class="cards">
			<div class="card card--3">
				<div class="card__wrapper">
					<img src="./assets/card3.jpg" alt="изображение">
				</div>
				
			</div>
			<div class="card card--2">
				<div class="card__wrapper">
					<img src="./assets/card2.jpg" alt="изображение">
				</div>
			</div>
			<div class="card card--1">
				<div class="card__wrapper">
					<img src="./assets/card1.jpg" alt="изображение">
				</div>
			</div>
		</div>
	</div>
</template>

<script>

export default {
	name: 'app',
	components: {
	}
}
</script>

<style lang="stylus">
borderWidth = 2px

*
	box-sizing border-box
html
	background-color #0E1215
#app
	margin 100px auto
	width 600px
.cards
	display flex
	justify-content center
	align-items center
	height 600px
.card
	width 167px
	margin-left -10px
	border solid #000 
	border-width borderWidth 
	background-color #282828
	&--1
		z-index 1
		height 440px
	&--2
		z-index 2
		height 470px
	&--3
		z-index 3
		height 500px
	&:hover
		z-index 4
		cursor pointer
		transform scale(1.2, 1.2)
		box-shadow 0 0 10px #979797
		border 0px
	&__wrapper
		border solid @border-width #979797
		// border solid borderWidth #000
		width 100%
		height 100%
</style>
