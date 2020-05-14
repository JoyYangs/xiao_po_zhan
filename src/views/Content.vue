<template>
	<div id="content">
		<div class="content1">
			<div class="content1-item left">
				<div class="left-item" v-for="item in leftItems" :key="item">
					<div class="img"></div>
					<div class="text">{{item}}</div>
				</div>
			</div>
			<div class="content1-item center">
				<a class="center-item" v-for="item of items" :key="item.name">
					<div>{{item.name}} <span v-if="item.count">{{item.count}}</span></div>
				</a>
			</div>
			<div class="content1-item right">
			</div>
		</div>
		<div class="content2"></div>
	</div>
</template>

<script>
export default {
	name: "Content",
	data() {
		return {
			leftItems: ["首页","关注","排行榜"],
			items: [{
				name: "动画",
				count: "999+"
			},{
				name: "番剧",
				count: "133"
			},{
				name: "音乐",
				count: "999+"
			},{
				name: "国创",
				count: "277"
			},{
				name: "舞蹈",
				count: "913"
			},{
				name: "游戏",
				count: "999+"
			},{
				name: "科技",
				count: "999+"
			},{
				name: "美食圈",
				count: "999+"
			},{
				name: "数码",
				count: "897"
			},{
				name: "生活",
				count: "999+"
			},{
				name: "鬼畜",
				count: "555"
			},{
				name: "时尚",
				count: "284"
			},{
				name: "资讯",
				count: "999+"
			},{
				name: "娱乐",
				count: "999+"
			},{
				name: "影视",
				count: "555"
			},{
				name: "放映厅",
				count: "238"
			},{
				name: "搞笑",
				count: "999+"
			},{
				name: "动物圈",
				count: "555"
			},{
				name: "单机游戏",
				count: "999+"
			},{
				name: "VLOG",
				count: ""
			}]

		}
	}
}
</script>

<style scoped>
a {
	color: black;
	font-size: 14px;
}
.content1 {
	padding: 15px 0;
	/* background-color: antiquewhite; */
	height: 70px;
	display: flex;
}

.content1 .left {
	width: 15%;
	display: flex;
	/* background-color: aquamarine; */
}

.content1 .left .left-item {
	flex: 1;
	display: flex;
	flex-direction: column;
	align-items: center;
	text-align: center;
	font-size: 14px;
}

.content1 .left .left-item .img{
	width: 40px;
	height: 40px;
	border-radius: 50%;
	background-color: antiquewhite;
}


.content1 .center {
	flex: 1;
	display: flex;
	flex-wrap: wrap;
	margin-left: 5px;
	padding-left: 5px;
	border-left: 1px solid #dddddd;
	border-right: 1px solid #dddddd;
}

.center-item div {
	flex: 1;
	margin: 5px 8px;
}

.center-item div span {
	background-color: #73CAE5;
	padding: 0px 5px;
	border-radius: 2px;
	font-size: 12px;
	color: #ffffff;
}

.content1 .right {
	width: 20%;
	/* background-color: beige; */
}
</style>