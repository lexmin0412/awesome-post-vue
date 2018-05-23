<template>
  <div class="left-nav"> 
		<ul>
			<li>
				<i class="icon iconfont icon-shumashouji"></i>
				<div>商品</div>
			</li>
			<li>
				<i class="icon iconfont icon-tianmaopaidui"></i>
				<div>店铺</div>
			</li>
			<li>
				<i class="icon iconfont icon-fenlei"></i>
				<div>统计</div>
			</li>
			<li>
				<i class="icon iconfont icon-shoucang"></i>
				<div>收藏</div>
			</li>
		</ul>
	</div>
</template>

<script>
export default {
    
}
</script>

<style>
	.left-nav {
		float: left;
		width: 8%;
		height: 100%;
		background-color: #1d8ce0;
		font-size: 10px;
		color: #fff;
	}
	.icon-font {
		font-size: 24px;
	}
	.left-nav ul {
		padding: 0;
		margin: 0;
	}
	.left-nav li {
		list-style-type: none;
		border-bottom: 1px solid #ebebeb;
		padding: 10px;
		text-align: center;
	}
</style>
