<template>
	<div id="header">
		<div class="bg-img">
			<img src="http://i0.hdslb.com/bfs/archive/ed92db305ae43c7fc8a59b1789934caa2636b876.png" alt="">
		</div>
		<div class="icon">
			<img src="http://i0.hdslb.com/bfs/archive/4de86ebf90b044bf9ba2becf042a8977062b3f99.png" alt="">
		</div>
	</div>
</template>

<script>
export default {
	name: "HomeHeader"
}
</script>

<style scoped>
	#header  {
		position: relative;
		width: 100vw;
	}

	.bg-img {
		max-width: 100%;
		background-position: center 0;
	}

	.icon {
		position: absolute;
		bottom: 10px;
		left: 100px;
	}
</style>