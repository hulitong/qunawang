<template>
  <div class="header">
 		<div class="header-left">
 			<span class="iconfont">&#xe624;</span>
 		</div>
 		<div class="header-input">
 			<span class="iconfont search-icon">&#xe632;</span>
 			输入城市/景点/游玩主题
 		</div>
 		<router-link to='/city'>
	 		<div class="header-city">
	 			{{this.city}}<span class="iconfont sj-icon">&#xe64a;</span>
	 		</div>
 		</router-link>
  </div>
</template>

<script>
export default {
  name: 'HomeHeader',
  props:{
  	city: String
  }
}
</script>

<style lang="stylus" scoped>
	@import '~styles/varibles.styl'
	.header
		display:flex
		width:100%
		height:.86rem
		background:$bgColor
		color:#fff
		.header-left
			float:left
			width:.64rem
			line-height:.86rem
			text-align:center
		.header-input
			flex:1
			background:#fff
			color:#666
			border-radius:.1rem
			height:.64rem
			line-height:.64rem
			padding-left:.2rem
			margin-top:.12rem
		  // margin-left:.2rem
		.header-city
			display:block
			width:1.23rem
			float:right
			line-height:.86rem
			text-align:center
			color:#fff
			.sj-icon
				font-size:.2rem
					
</style>