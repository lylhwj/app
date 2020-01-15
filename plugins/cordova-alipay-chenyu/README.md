#插件简介

  1.插件提供支付宝支付
  <br>
  2.本插件是基于cordova开发的支付宝支付插件，
  凡是基于cordova的webapp项目就可以调用本插件
  <br>
  3.插件提供js调用方式。并且提供angular/ionic2、3项目ts调用方式
  <br>
  4.你们支持是我们的开发动力、如果调用问题请联系我们

#安装使用:


     1. cordova-android@6.4.0 以下的请使用 cordova plugin add cordova-alipay-chenyu@1.1.2 --variable APP_ID=你的支付宝id
     2. cordova-android@7.0.0 以上的请使用 cordova plugin add cordova-alipay-chenyu --variable APP_ID=你的支付宝id


#调用说明（js方式）：

    ### //签名字符串
    let orderStr="";
    cordova.plugins.MyAlipay.coolMethod(orderStr,
      (msg) => {
        // console.log("msg:"+msg);
      },
      (msg) => {
        alert('失败');
      }
    );

#返回参数：
返回结果示例 iOS|Android

    {
       "memo" : "xxxxx",
       "result" : "{
                       \"alipay_trade_app_pay_response\":{
                           \"code\":\"10000\",
                           \"msg\":\"Success\",
                           \"app_id\":\"2014072300007148\",
                           \"out_trade_no\":\"081622560194853\",
                           \"trade_no\":\"2016081621001004400236957647\",
                           \"total_amount\":\"0.01\",
                           \"seller_id\":\"2088702849871851\",
                           \"charset\":\"utf-8\",
                           \"timestamp\":\"2016-10-11 17:43:36\"
                       },
                       \"sign\":\"NGfStJf3i3ooWBuCDIQSumOpaGBcQz+aoAqyGh3W6EqA/gmyPYwLJ2REFijY9XPTApI9YglZyMw+ZMhd3kb0mh4RAXMrb6mekX4Zu8Nf6geOwIa9kLOnw0IMCjxi4abDIfXhxrXyj********\",
                       \"sign_type\":\"RSA2\"
                   }",
       "resultStatus" : "9000"
    }
  <br>
  [详情参考支付宝文档](https://docs.open.alipay.com/204/105301/)
  <br>
<br>
#ionic2、3调用方式（ts方式）:
参考地址：https://www.npmjs.com/package/cordova-alipay-chenyu-ionic

#联系我们
QQ:250187715
<br>
QQ群:390736068