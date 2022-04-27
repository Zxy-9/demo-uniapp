<template>
    <view>
        <u-grid >
            <u-grid-item v-for="(baseListItem,baseListIndex) in baseList"
                    :key="baseListIndex"
					@click="clickIcon(baseListIndex)">
				<i class="iconfont" :class="baseListItem.name"></i>		
                <text class="grid-text">{{baseListItem.title}}</text>
            </u-grid-item>
        </u-grid>
		
        <u-toast ref="uToast" />
    </view>
</template>

<script>
    export default {
        data() {
            return {
                baseList: [{
                    name: 'icon-icon',
                    title: '纪念日'
                    },
                    {
                        name: 'icon-icon',
                        title: '锁头'
                    },
                    {
                        name: 'icon-icon',
                        title: '星星'
                    },
                ]
            }
        },
        methods: {
            clickIcon(baseListIndex){
             //   this.$refs.uToast.success(`点击了${baseListIndex}`)
			 if(baseListIndex == 0)
				uni.navigateTo({
					url:'../memorialDay/index'
				})
				
            }
        }
    }
</script>

<style lang="scss">
    .grid-text {
        font-size: 14px;
        color: #909399;
        padding: 10rpx 0 20rpx 0rpx;
        /* #ifndef APP-PLUS */
        box-sizing: border-box;
        /* #endif */
    }
	.iconfont{
		margin-top: 30rpx;
	}
</style>