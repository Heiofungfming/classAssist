<template>
	<view>
    <tui-navigation-bar title="班级助手" 
      color="#fff"
      backgroundColor="#5677fc"
      :isOpacity="false"></tui-navigation-bar>
		<view class="content">
      个人信息
		</view>
    <!-- <tui-tabbar :current="current"  
      backdropFilter 
      :tabBar="tabBar" 
      color="#777" 
      selectedColor="#5677fc"
      :hump="true"
      @click="tabbarSwitch"></tui-tabbar> -->
	</view>
</template>

<script>
	export default {
		data() {
			return {
				current: 2
				// tabBar: [
        //   {
        //     pagePath: '/pages/home/index',
        //     text: '首页',
        //     iconPath: '/static/image/tabbar/home.png',
        //     selectedIconPath: '/static/image/tabbar/home-fill.png'
        //   },
        //   {
        //     pagePath: '',
        //     text: '添加',
        //     iconPath: '/static/image/tabbar/add.png',
        //     hump: true,
        //     selectedIconPath: '/static/image/tabbar/add-fill.png'
        //   },
        //   {
        //     pagePath: '/pages/self/index',
        //     text: '个人',
        //     iconPath: '/static/image/tabbar/me.png',
        //     selectedIconPath: '/static/image/tabbar/me-fill.png',
        //     num: 2,
        //     isDot: true,
        //     verify: true
        //   }
        // ]
			}
		},
		onLoad() {
		},
		methods: {
      tabbarSwitch(obj) {
        let { pagePath } = obj
        uni.navigateTo({
          url: pagePath
        })
      }
		}
	}
</script>

<style>

</style>
