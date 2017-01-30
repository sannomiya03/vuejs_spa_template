<template lang="pug">
	div
		appHeader.app-header
		router-view.app-body
</template>
<script lang="coffee">
	module.exports =
		components:
			appHeader: require "./components/header"
</script>
<style lang="stylus">
	@import "~stylus/setting"

	html, body
		position relative
		width 100%
		height 100%
		background-color appBgColor

	.app-header
		height headerHeight
		display flex
		align-items center
		background-color White
		border-bottom 1.5px solid Gray300
		z-index 8000

	.app-body
		position relative
</style>