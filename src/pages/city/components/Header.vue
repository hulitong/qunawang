<template>
	<div class="header-city">
		<router-link to="/">
			<span class="iconfont city-back">&#xe624;</span>
		</router-link>
		城市
	</div>
</template>
<script>
export default {
	name: 'CityHeader'
}	
</script>
<style lang="stylus" scoped>
	@import '~styles/varibles.styl'
	.header-city
		height:$headerHeight
		line-height:$headerHeight
		background:$bgColor
		color:#fff
		text-align:center
		font-size:.42rem
		.city-back
			position:absolute
			top:0
			left:.1rem
			color:#fff
</style>