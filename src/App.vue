<template>
	<div id="app">
		<transition name="fade" mode="out-in">
			<router-view></router-view>
		</transition>
	</div>
</template>

<script>

export default {
	name: 'app',
	data() {
        return {
            breadcrumbs:[{name:'首页',path:'/'}]
        }
    },
	 methods: {
    },
}

</script>

<style lang="scss">
body {
    margin: 0px;
    padding: 0px;
    // background: url(./assets/img/bg1.jpg) center !important;
    background-size: cover;
    // background: #1F2D3D;
    font-family: Helvetica Neue, Helvetica, PingFang SC, Hiragino Sans GB, Microsoft YaHei, SimSun, sans-serif;
    font-size: 14px;
    -webkit-font-smoothing: antialiased;
}

#app {
	position: absolute;
	top: 0px;
	left:0px;
	bottom: 0px;
	width: 100%;
}



.fade-enter-active,
.fade-leave-active {
	transition: all .1s ease;
}

.fade-enter,
.fade-leave-active {
	opacity: 0;
}

</style>
