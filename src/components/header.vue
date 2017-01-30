<template lang="pug">
	header.main-header
		h1.site-title {{site.siteTitle}}
</template>
<script lang="coffee">
	module.exports =
		data: -> return { site: require "scripts/site_info" }
</script>
<style lang="stylus" scoped>
	@import "~stylus/setting"
	
	.main-header
		height headerHeight
</style>
