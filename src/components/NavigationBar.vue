<template>
	<div id="nav-bar">
		<div class="top-titles left">
			<a href="https://app.bilibili.com/" class="title-item" target="_blank" v-for="title of titles.left" :key="title">
				<span>{{title}}</span>
			</a>
		</div>
		<div class="top-titles top-input">
			<input class="input" type="text" placeholder="Hiphop女孩VS百褶裙女孩">
			<div class="search">🔍</div>
		</div>
		<div class="top-titles right">
			<div class="title-item" v-for="title of titles.right" :key="title">{{title}}</div>
			<div class="tougao">投稿</div>
		</div>
		
	</div>
</template>

<script>
export default {
	name: "NavigationBar",
	props: {
		titles: {
			type: Object,
			default: {}
		}
	}
}
</script>

<style scoped>
#nav-bar {
	width: 100%;
	height: 56px;
	font-size: 14px;
	color: #ffffff;
	display: flex;
}
.top-titles {
	flex: 1;
	margin: 9px;
	height: 38px;
	line-height: 38px;
	display: flex;
	justify-content: space-evenly;
}

.top-input {
	border-radius: 4px;
	background-color: #ffffff;
}

.input {
	flex: 1;
	padding: 0 10px;
	outline-style: none;
	border: none;
}
.search {
	width: 60px;
	color: black;
	text-align: center;
	background-color: #cccccc;
}

.tougao {
	background-color: #FB7299;
	width: 100px;
	height: 36px;
	text-align: center;
	line-height: 36px;
	border-radius: 4px;
}

</style>