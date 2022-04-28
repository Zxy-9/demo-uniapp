<template>
	<view class="container">
		<scroll-view>
			<view class="img_container">
				<view class="img_text">
					<u--text  text="距离" color = '#efefef'></u--text>
					<u--text text="中秋节" color = '#efefef'></u--text>
					<u--text text="144" size=25 color = '#efefef'></u--text>
					<text style="color: #efefef;">天</text>
				</view>
			</view>
			<view class="list_container">
				<ul>
					<li >
						<view class="list_list">
							<view class="list_line"></view>
							<view class="list_title">
							 <h4>春节</h4>
							 <text>3月28日</text>
							</view>
							<view class="list_day">
								<text>还有<text class="day">144</text>天 </text>
							</view>
						</view>
					</li>
					<li>
						<view class="list_list">
							
						</view>
					</li>
				</ul>
				
			</view>
		</scroll-view>
		
		
	</view>
</template>

<script>
	export default{
		data(){
			return{
				
			}
		}
	}
</script>

<style>
	.container{
		padding: 50rpx;
	}
	.img_container{
		height: 300rpx;
		width: 100%;
		float: none;
		background-color: #0077AA;
	}
	.list_container{
		width: 90%;
		height: auto;
		margin-top: -50rpx;
		z-index: 100;
		margin-left:5%;
	}
	ul{
		list-style: none;
		padding: 0;
	}
	.list_list{
		width:100%;
		border-radius: 10rpx;
		height: 150rpx;
		margin-top: 20rpx;
		display: flex;
		border: 1px solid #D9D9D6;
		background-color: white;
		box-shadow: 5rpx 5rpx 5rpx #efefef;
		z-index: 999;
	}
	.list_line{
		background-color: red;
		height: 150rpx;
		width: 10rpx;
		border-radius: 10rpx 0 0 10rpx;
		background-image: linear-gradient(#2DCCD3,#00B140);
	}
	.list_title{
		padding: 30rpx;
	}
	.list_day .day{
		font-size: 25px;
		color: #0077AA;
		margin: 0 15rpx 0 15rpx;
	}
	.list_day{
		padding-top: 40rpx;
		margin-left: 140rpx;
		
		
	}
</style>
