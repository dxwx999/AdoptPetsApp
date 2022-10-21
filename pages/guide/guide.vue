<template>
  <view class="guide_container">
    <view class="status_bar">
        <!-- 这里是状态栏 -->
    </view>
    <!-- 指引页面标题-->
    <view class="guide_top_text">在这里，你可以找到合适你的那个它</view>
    <!-- 指引页面小字-->
    <view class="guide_middle_text">
      这里有各种各样的宠物，以及它们需要的宠物配件
    </view>
    <view class="guide_background">
    </view>
    <!-- 通过navigator跳转到登录页面-->
    <navigator url="/pages/login/login" class="guide_next">
      <image src="/static/guide_next.png"></image>
    </navigator>  
  </view>
</template>

<script>
  export default {
    data() {
      return { 
      };
    },  
  }
</script>

<style lang="less">
  .status_bar {
      height: var(--status-bar-height);
      width: 100%;
  }
  .guide_container{

     .guide_top_text{
        position: absolute;
        left: 54rpx;
        top: 180rpx;
        width: 642rpx;
        height: 212rpx;
        opacity: 1;
        /** 文本1 */
        font-size: 70rpx;
        font-weight: 700;
        letter-spacing: 0rpx;
        line-height: 105.92rpx;
        color: rgba(46, 37, 37, 1);
        text-align: left;
        vertical-align: top;
      }
      .guide_middle_text{
        position: absolute;
        left: 54rpx;
        top: 500rpx;
        width: 642rpx;
        height: 142rpx;
        opacity: 1;
        /** 文本1 */
        font-size: 36rpx;
        font-weight: 400;
        letter-spacing: 0.72rpx;
        line-height: 60.22rpx;
        color: rgba(46, 37, 37, 0.7);
        text-align: left;
        vertical-align: top;
      }
      .guide_background{
        position: absolute;  //决定定位，这里的绝对定位是相对于html进行定位的
        width:750rpx;  //微信小程序的单位，用于移动端适配
        height: 393.75rpx;
        background: url(/static/guide_background.png) ;
        background-size:cover;
        left: 0rpx;
        bottom: 254rpx;
      }
      .guide_next{
        image{
          position: absolute;
          right: 34rpx;
          bottom: 34rpx;
          width: 165.06rpx;
          height: 165.06rpx;
        }
      }
  }
 
</style>
