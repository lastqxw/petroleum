<script>
	export default {
		onShow() {
			// 调用API从本地缓存中获取数据
			const logs = wx.getStorageSync('logs') || []
			logs.unshift(Date.now())
			wx.setStorageSync('logs', logs)
      wx.showShareMenu()
		}
  }
</script>

<style>
	.container {
		height: 100%;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: space-between;
		padding: 200rpx 0;
		box-sizing: border-box;
	}

	page {
		background-color: #efeff4;
		/* height: 100%;
		-webkit-overflow-scrolling: touch; */
		
		
	}

	/* this rule will be remove */
	* {
		transition: width 2s;
		-moz-transition: width 2s;
		-webkit-transition: width 2s;
		-o-transition: width 2s;
	}
</style>
