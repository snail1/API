# API
前端常用api

UC 浏览器的部分私有Meta 属性
1、<meta name="imagemode" content="force">无图模式强制显示图片
2、<meta name="full-screen" content="yes">强制浏览器全屏
3、<meta name="viewport" content="uc-fitscreen=no|yes>缩放不出滚动条

1、<meta http-equiv="refresh" content="0;url=" />
页面重定向和刷新
2、<meta name="apple-mobile-web-app-capable" content="yes" /> 启用 WebApp 全屏模式
3、<meta name="apple-itunes-app" content="app-id=432274380"> 下载广告条

3、<meta name="apple-mobile-web-app-status-bar-style" content="black-translucent" />隐藏状态栏/设置状态栏颜色：只有在开启WebApp全屏模式时才生效。content的值为default | black | black-translucent 。
4、<meta name="apple-mobile-web-app-title" content="标题">添加到主屏后的标题
5、<meta content="telephone=no" name="format-detection" /> 忽略数字自动识别为电话号码
6、<meta content="email=no" name="format-detection" />忽略识别邮箱
7、<meta http-equiv="Pragma" content="no-cache">禁止浏览器从本地计算机的缓存中访问页面内容
8、<meta name="apple-mobile-web-app-capable" content="yes"/>通过safari浏览该html的时候保存的Cookie等其他数据不会被清空
9、<meta name="apple-mobile-web-app-status-bar-style" content="black" />改变顶部状态条的颜色
10、<link rel="apple-touch-icon-precomposed" href="iphone_logo.png" /> Web App 的放置主屏幕上 icon 文件路径
11、<meta http-equiv="Expires" content="-1"> 用于设定网页的到期时间过期则必须到服务器上重新调用 content="-1"，网页在任何时候都不能被Cache存储
12、<meta http-equiv="Window-target" content="_top"> 强制页面在当前窗口以独立页面显示。注意：用来防止别人在框架里调用自己的页面。
13、<meta name="applicable-device" content="mobile">在移动的响应的包头中添加
14、<meta name="screen-orientation" content="portrait"><!-- uc强制竖屏 -->
15、<meta name="x5-orientation" content="portrait">      <!-- QQ强制竖屏 --> 
16、<link href="/startup.png" rel="apple-touch-startup-image" />   给Web App加上一个启动界面
<!doctype html>
<!-- http://taylor.fausak.me/2015/01/27/ios-8-web-apps/ -->

<html>
  <head>
    <title>iOS 8 web app</title>

    <!-- CONFIGURATION -->

    <!-- Allow web app to be run in full-screen mode. -->
    <meta name="apple-mobile-web-app-capable"
          content="yes">

    <!-- Make the app title different than the page title. -->
    <meta name="apple-mobile-web-app-title"
          content="iOS 8 web app">

    <!-- Configure the status bar. -->
    <meta name="apple-mobile-web-app-status-bar-style"
          content="black">

    <!-- Set the viewport. -->
    <meta name="viewport"
          content="initial-scale=1">

    <!-- Disable automatic phone number detection. -->
    <meta name="format-detection"
          content="telephone=no">

    <!-- ICONS -->

    <!-- iPad retina icon -->
    <link href="https://placehold.it/152"
          sizes="152x152"
          rel="apple-touch-icon-precomposed">

    <!-- iPad retina icon (iOS < 7) -->
    <link href="https://placehold.it/144"
          sizes="144x144"
          rel="apple-touch-icon-precomposed">

    <!-- iPad non-retina icon -->
    <link href="https://placehold.it/76"
          sizes="76x76"
          rel="apple-touch-icon-precomposed">

    <!-- iPad non-retina icon (iOS < 7) -->
    <link href="https://placehold.it/72"
          sizes="72x72"
          rel="apple-touch-icon-precomposed">

    <!-- iPhone 6 Plus icon -->
    <link href="https://placehold.it/180"
          sizes="120x120"
          rel="apple-touch-icon-precomposed">

    <!-- iPhone retina icon (iOS < 7) -->
    <link href="https://placehold.it/114"
          sizes="114x114"
          rel="apple-touch-icon-precomposed">

    <!-- iPhone non-retina icon (iOS < 7) -->
    <link href="https://placehold.it/57"
          sizes="57x57"
          rel="apple-touch-icon-precomposed">

    <!-- STARTUP IMAGES -->

    <!-- iPad retina portrait startup image -->
    <link href="https://placehold.it/1536x2008"
          media="(device-width: 768px) and (device-height: 1024px)
                 and (-webkit-device-pixel-ratio: 2)
                 and (orientation: portrait)"
          rel="apple-touch-startup-image">

    <!-- iPad retina landscape startup image -->
    <link href="https://placehold.it/1496x2048"
          media="(device-width: 768px) and (device-height: 1024px)
                 and (-webkit-device-pixel-ratio: 2)
                 and (orientation: landscape)"
          rel="apple-touch-startup-image">

    <!-- iPad non-retina portrait startup image -->
    <link href="https://placehold.it/768x1004"
          media="(device-width: 768px) and (device-height: 1024px)
                 and (-webkit-device-pixel-ratio: 1)
                 and (orientation: portrait)"
          rel="apple-touch-startup-image">

    <!-- iPad non-retina landscape startup image -->
    <link href="https://placehold.it/748x1024"
          media="(device-width: 768px) and (device-height: 1024px)
                 and (-webkit-device-pixel-ratio: 1)
                 and (orientation: landscape)"
          rel="apple-touch-startup-image">

    <!-- iPhone 6 Plus portrait startup image -->
    <link href="https://placehold.it/1242x2148"
          media="(device-width: 414px) and (device-height: 736px)
                 and (-webkit-device-pixel-ratio: 3)
                 and (orientation: portrait)"
          rel="apple-touch-startup-image">

    <!-- iPhone 6 Plus landscape startup image -->
    <link href="https://placehold.it/1182x2208"
          media="(device-width: 414px) and (device-height: 736px)
                 and (-webkit-device-pixel-ratio: 3)
                 and (orientation: landscape)"
          rel="apple-touch-startup-image">

    <!-- iPhone 6 startup image -->
    <link href="https://placehold.it/750x1294"
          media="(device-width: 375px) and (device-height: 667px)
                 and (-webkit-device-pixel-ratio: 2)"
          rel="apple-touch-startup-image">

    <!-- iPhone 5 startup image -->
    <link href="https://placehold.it/640x1096"
          media="(device-width: 320px) and (device-height: 568px)
                 and (-webkit-device-pixel-ratio: 2)"
          rel="apple-touch-startup-image">

    <!-- iPhone < 5 retina startup image -->
    <link href="https://placehold.it/640x920"
          media="(device-width: 320px) and (device-height: 480px)
                 and (-webkit-device-pixel-ratio: 2)"
          rel="apple-touch-startup-image">

    <!-- iPhone < 5 non-retina startup image -->
    <link href="https://placehold.it/320x460"
          media="(device-width: 320px) and (device-height: 480px)
                 and (-webkit-device-pixel-ratio: 1)"
          rel="apple-touch-startup-image">

    <!-- HACKS -->

    <!-- Prevent text size change on orientation change. -->
    <style>
      html {
        -webkit-text-size-adjust: 100%;
      }
    </style>
  </head>

  <body>
    <h1>iOS 8 web app</h1>
  </body>
</html>





17、<input autocorrect=”off” autocomplete=”off” autocapitalize=”off”> 关闭iOS中键盘自动大写、自动更正、自动完成
18、<a href="sms:18888886666,18888885555″]]> 发送短信给多个人 的链接
19、<a href="sms:18888886666?body=sms txt"]]> 发送短信附带内容 的链接
20、<a href="tel:18888886666"]]>Call us at 18888886666</a]]> 拨打电话的链接

21、<input type="button" value="Go Full screen"  onclick='document.querySelector("video").webkitEnterFullScreen()'>video元素的全屏播放

22、input::-webkit-input-placeholder{color:#AAAAAA;}
input:focus::-webkit-input-placeholder{color:#EEEEEE;}webkit表单输入框placeholder的颜色值能改变么


23、网站变黑白-webkit-filter: grayscale(100%);

24、<meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1" /> 优先使用最新版本 IE 和 Chrome

响应式图片
	
<img src="lores.png" srcset="hires.png 2x, superhires.png 3x">



默认样式更改
a, img { -webkit-touch-callout: none;   }/*禁止长按链接与图片弹出菜单*/
html, body { -webkit-user-select: none;user-select: none;}  /* 禁止选中文本（如无文本选中需求，此为必选项）*/
-webkit-tap-highlight-color:rgba(200,0,0,0.4)自定义高亮颜色
input {-webkit-appearance:none; /*去除input默认样式*/}
-webkit-text-size-adjust: none; //禁止文字自动调整大小(

背景模糊	filter: blur(0.8);
	-webkit-filter:blur(5px);



ios和android局部滚动时隐藏原生滚动条
::-webkit-scrollbar{
    opacity: 0;
}
滚动条

::-webkit-scrollbar-track-piece{ 
background-color:#fff;/*滚动条的背景颜色*/ 
-webkit-border-radius:0;/*滚动条的圆角宽度*/ 
} 
::-webkit-scrollbar{ 
width:8px;/*滚动条的宽度*/ 
height:8px;/*滚动条的高度*/ 
} 
::-webkit-scrollbar-thumb:vertical{/*垂直滚动条的样式*/ 
height:50px; 
background-color:#999; 
-webkit-border-radius:4px; 
outline:2pxsolid#fff; 
outline-offset:-2px; 
border:2pxsolid#fff; 
} 
::-webkit-scrollbar-thumb:hover{/*滚动条的hover样式*/ 
height:50px; 
background-color:#9f9f9f; 
-webkit-border-radius:4px; 
} 
::-webkit-scrollbar-thumb:horizontal{/*水平滚动条的样式*/ 
width:5px; 
background-color:#CCCCCC; 
-webkit-border-radius:6px; 
} 



.wx-code::-webkit-scrollbar{width:8px;height:8px}
.wx-code::-webkit-scrollbar-thumb{background-color:#2274e6;border-radius:4px}
.wx-code::-webkit-scrollbar-track{border-radius:4px;background:#eee}



边框0.5解决办法
.Suspend .car:before ,.Suspend .service:before {
	content: '';
    position: absolute;
    top: -50%;
    bottom: -50%;
    left: -50%;
    right: -50%;
    -webkit-transform: scale(0.5);
    transform: scale(0.5);
    border-right: 1px solid #cccccc;
}

.border-image-1px {
    border-width: 1px 0px;
    -webkit-border-image: url("data:image/png;base64,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") 2 0 stretch;
}

.scale{
    position: relative;
}
.scale:after{
    content:"";
    position: absolute;
    bottom:0px;
    left:0px;
    right:0px;
    border-bottom:1px solid #ddd;
    -webkit-transform:scaleY(.5);
    -webkit-transform-origin:0 0;
}







chrome下样式黄色的清除
input:-webkit-autofill {
	-webkit-box-shadow: 0 0 0px 1000px white inset;
	border: 1px solid #CCC!important;
}



1. 禁止右键点击
$(document).ready(function(){
    $(document).bind("contextmenu",function(e){
        return false;
    });
});
2.没找到图片
$('img').on('error', function () {
  $(this).prop('src', 'img/broken.png');
});

判断是否是web app状态。是否是苹果机型！

if (window.navigator.userAgent.indexOf('iPhone') != -1) {
        if (window.navigator.standalone == true) {
                alert("是苹果，已经加入到桌面");
        } else { 
                alert("没有加入！");
        };
} else {
        alert("不是苹果");
        //document.location.href = 'please-open-from-an-iphone.html';
};


重力感应
if (window.DeviceMotionEvent) { 
         window.addEventListener('devicemotion',deviceMotionHandler, false);  
} 
var speed = 30;//speed
var x = y = z = lastX = lastY = lastZ = 0;
function deviceMotionHandler(eventData) {  
  var acceleration =event.accelerationIncludingGravity;
        x = acceleration.x;
        y = acceleration.y;
        z = acceleration.z;
        if(Math.abs(x-lastX) &gt; speed || Math.abs(y-lastY) &gt; speed || Math.abs(z-lastZ) &gt; speed) {
            //简单的摇一摇触发代码
            alert(1);
        }
        lastX = x;
        lastY = y;
        lastZ = z;
}


WeixinApi.ready		
<div id="WeixinJsApi">
    <input type="button" id="toggleMenuBtn" value="隐藏右上角按钮">
    <input type="button" id="toggleToolbar" value="隐藏底部导航栏">
    <input type="button" id="getNetType" value="获取网络状态">
</div>

var menuHidden = false;
var toolbarHidden = false;
var netType = {
	"network_type:wifi": "wifi网络",
	"network_type:edge": "非wifi,包含3G/2G",
	"network_type:fail": "网络断开连接",
	"network_type:wwan": "2g或者3g"
};
document.addEventListener("WeixinJSBridgeReady", function onBridgeReady() {
	document.getElementById("toggleMenuBtn").addEventListener("click", function(a) {
		if(!menuHidden) {
			WeixinJSBridge.call("hideOptionMenu");
			menuHidden = true;
			this.value = "显示右上角按钮"
		} else {
			WeixinJSBridge.call("showOptionMenu");
			menuHidden = false;
			this.value = "隐藏右上角按钮"
		}
	}, false);
	document.getElementById("toggleToolbar").addEventListener("click", function(a) {
		if(!toolbarHidden) {
			WeixinJSBridge.call("hideToolbar");
			toolbarHidden = true;
			this.value = "显示底部导航栏"
		} else {
			WeixinJSBridge.call("showToolbar");
			toolbarHidden = false;
			this.value = "隐藏底部导航栏"
		}
	}, false);
	document.getElementById("getNetType").addEventListener("click", function(a) {
		WeixinJSBridge.invoke("getNetworkType", {}, function(b) {
			alert(netType[b.err_msg])
		})
	}, false)
});




wiso


网页是否在微信中被调用

var ua = navigator.userAgent.toLowerCase();
if(ua.match(/MicroMessenger/i)=="micromessenger") {

}else {
   alert("调用失败，请用微信扫一扫，扫描下面二维码打开网页！");
}



使用js禁止用户选中网页上的内容，IE及Chrome下的方法一样。
<body onselectstart="return false">


将彻底屏蔽鼠标右键
oncontextmenu=”window.event.returnValue=false”
< table border oncontextmenu=return(false)>< td>no< /table> 可用于 Table


禁止网页被人IFRAME套用
<SCRIPT LANGUAGE=JAVASCRIPT>
var url=window.location.href;
if(window!=parent)
parent.navigate(url);
</SCRIPT> 


调试
/*$("html").on("tap",function(e){
    console.log(e.target);
    console.log(e.target);
    /*console.info('信息');
    console.error('错误');
    console.warn('警告');
})*/



分散对齐
.info-title{
   text-align: justify;
}
.info-title:after{
   content: '';
   display: inline-block;
   width: 100%;
   height: 0;
   line-height: 0;
}
