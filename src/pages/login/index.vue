<template>
	<view>
    <tui-navigation-bar title="班级助手" 
      color="#fff"
      backgroundColor="#5677fc"
      :isOpacity="false"></tui-navigation-bar>
		<view class="content">
      <view class="btn_box">
        <tui-button width="692rpx"
          shape="circle"
          style="margin-top:30px">创建班级</tui-button>
        <tui-button width="692rpx" 
          shape="circle" 
          plain
          style="margin-top:20px"
          @click="joinClass">加入班级</tui-button>
      </view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
		onLoad() {
      // uni.showTabBar()
		},
		methods: {
      joinClass() {
        uni.switchTab({
          url: '/pages/home/index'
        })
      }
		}
	}
</script>

<style>
  .btn_box {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
</style>
