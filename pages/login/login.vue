<template>
  <view class="login_container">
    <view class="login_title">
      <image src="/static/login/topPet.png" mode="" class="title_img"></image>
      <text>快来带我回家吧~</text>
    </view>
    <view class="login_bakground">
      <view class="login_change">
        <view class="login_btn">
          登录
        </view>
        <view class="reg_btn">
          注册
        </view>
      </view>
      <view class="input_view">
        <!-- 手机号输入区域-->
        <view class="login_phoneNum login_input_box" >
          <i class="icon icon-shouji input_icon"></i>
          <text>手机号</text>
          <input class="uni-input login_input" type="number" placeholder="请输入手机号" maxlength="11"/>
        </view>
        <!-- 密码输入区域-->
          <view class="login_verification login_input_box" >

            <input class="uni-input login_input" type="number" placeholder="请输入验证码" maxlength="6"/>
            <button type="default" class="get_verification">获取验证码</button>
          </view>
      </view>

          <!-- 登录按钮-->
           <button type="primary" class="loginBtn">登录</button>
           
           <!-- or区域-->
             <span class="otherLogin">其他登录方式</span>
            <!--其他登录区域-->
            <view class="otherWay">
              <i class="icon icon-weixin"></i>
              <i class="icon icon-QQ"></i>
              <i class="icon icon-weibo"></i>
            </view>
      </view>
      <!-- 注册区域结束-->
     
      
    </view>
  </view>
</template>

<script>
  export default {
    data() {
      return {
        
      };
    }
  }
</script>

<style lang="less">
.login_container{
  position: absolute;
  bottom: 0;
  width: 750rpx;
  height: 100vh;
  display: flex;
  flex-direction: column;
  background-color: rgba(253, 211, 0, 1);
    .login_title{
      flex: 1;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      .title_img{
        width: 148rpx;
        height: 178rpx;
        padding: 0 40rpx 40rpx 0;
      }
    }
  .login_bakground{
    flex:3;
    background-color:#F9F9F9;
    display: flex;
    flex-direction: column;
    border-radius: 68rpx 68rpx 0 0 ;
    .login_change{
      padding-top: 50rpx;
      height: 104rpx ;
      .login_btn{
        display: inline-block;
        font-size: 40rpx;
        font-weight: 600;
        position: relative;
        left: 38rpx;
        top: 20rpx;
        width: 130rpx;
        height: 54rpx;
        text-align: center;
      }
      .reg_btn{
        display: inline-block;
        position: relative;
        width: 130rpx;
        height: 34rpx;
        top:21rpx;
        color: rgba(12, 12, 14, 0.5);
        text-align: center;
        font-size: 28rpx;
        font-weight: 500;
        letter-spacing: 1.4rpx;
      }
    }
    .input_view{
      display: flex;
      flex-direction: column;
      align-items:center ;
      .login_verification{
        
        position: relative;
        width: 610rpx !important;
        justify-content: flex-start !important;
        input{
          padding-left: 40rpx;
        }
        button{
          color:gray;
        }
        .get_verification{
          background-color: #FFB801;
          color:white;
          position: absolute;
          right: 0;
          border-radius: 45rpx;
          height: 90rpx;
          margin:0 ;
        }
      }
        //输入框的定位
        .login_input_box{
          margin-bottom: 40rpx;
          width: 610rpx;
          height: 92rpx;
          background-color: white;
          border-radius:45rpx;
          line-height: 120rpx;
          display: flex;
          justify-content: space-around;
          align-items: center;
      
          .input_icon{
            // text-align: left;
            width: 50rpx;
            height: 50rpx;
          }
          .login_input{
            display: inline-block;
          }
        }
      }
     
    }
 
   .loginBtn{
     margin-top: 50rpx;
     width: 534.42rpx;
     height: 108.7rpx;
     background-color:#FFB801;
     border-radius: 18rpx;
   }
   
   .otherLogin{
     opacity: 50%;
     text-align: center;
     margin-top: 100rpx;
   }
   .otherLogin::before,
   .otherLogin::after{
     content: ' —— ';
   }
   
   .otherWay{
     display: flex;
     justify-content: space-around;
     padding: 100rpx 100rpx 0 100rpx;
     i{
       width: 80rpx;
       height: 80rpx;
     }
   }
  

}
</style>
