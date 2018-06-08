##  百度统计
```
<script>
var _hmt = _hmt || [];
(function() {
  var hm = document.createElement("script");
  hm.src = "https://hm.baidu.com/hm.js?2c681ae4f5f65e293c799beac90eedb7";
  var s = document.getElementsByTagName("script")[0];
  s.parentNode.insertBefore(hm, s);
})();
</script>
```
##  单页换公司及资质
```
<script>
$(function () {
    // 备案号列表
    var corporationList = [
        {
            "id":0,
            "name":"广州向荣教育科技有限公司",
            "num":"鄂ICP备12016896号-8"
        },{
            "id":1,
            "name":"湖北云天下教育科技有限公司",
            "num":"鄂ICP备12016896号-7"
        },{
            "id":2,
            "name":"武汉智慧环球科技有限公司",
            "num":"鄂ICP备16004339号-3"
        },{
            "id":3,
            "name":"武汉乐教科技有限公司",
            "num":"鄂ICP备13016533号"
        },{
            "id":4,
            "name":"北京文博华茂科技有限公司",
            "num":"京ICP备16065121号-1"
        },{
            "id":5,
            "name":"深圳市佩思维科技有限公司",
            "num":"粤ICP备15038492号-1"
        },{
            "id":6,
            "name":"惠州市宏茂网络科技有限公司",
            "num":"粤ICP备17014673号-1"
        },{
            "id":7,
            "name":"惠州优车宝网络科技有限公司",
            "num":"粤ICP备15101985号-1"
        },{
            "id":8,
            "name":"武汉智慧环球教育科技有限公司",
            "num":"鄂ICP备16004339号"
        },{
            "id":9,
            "name":"北京千才汇教科技有限公司",
            "num":"京ICP备16020172号-2"
        },{
            "id":10,
            "name":"北京文博华茂科技有限公司",
            "num":"京ICP备16065121号"
        },{
            "id":11,
            "name":"武汉书香门第教育科技有限公司",
            "num":"鄂ICP备18009206号-1"
        },{
            "id":12,
            "name":"合肥盘手金融教育培训有限公司",
            "num":" "
        },{
            "id":13,
            "name":"长沙市亿泰科技有限公司",
            "num":"湘ICP备17018323号-3"
         }
    ];
    // 主域名
    var test = window.location.host;
    // 显示域名位置
    var $footer = $('.footer');
    // 更换域名
    if(test.indexOf('ytxedu') > 0){
        $footer.html('<p>Copyright © 2018 '+corporationList[0].name+' All Rights Reserved <br>'+corporationList[0].num+'</p>')
    }else if(test.indexOf('ykclass') > 0){
        $footer.html('<p>Copyright © 2018 '+corporationList[1].name+' All Rights Reserved <br>'+corporationList[1].num+'</p>')
    }else if(test.indexOf('guopass') > 0){
        $footer.html('<p>Copyright © 2018 '+corporationList[2].name+' All Rights Reserved <br>'+corporationList[2].num+'</p>')
    }else if(test.indexOf('topksw') > 0){
        $footer.html('<p>Copyright © 2018 '+corporationList[3].name+' All Rights Reserved <br>'+corporationList[3].num+'</p>')
    }else if(test.indexOf('yythb') > 0){
        $footer.html('<p>Copyright © 2018 '+corporationList[4].name+' All Rights Reserved <br>'+corporationList[4].num+'</p>')
    }else if(test.indexOf('peisway') > 0){
        $footer.html('<p>Copyright © 2018 '+corporationList[5].name+' All Rights Reserved <br>'+corporationList[5].num+'</p>')
    }else if(test.indexOf('hzhmcy') > 0){
        $footer.html('<p>Copyright © 2018 '+corporationList[6].name+' All Rights Reserved <br>'+corporationList[6].num+'</p>')
    }else if(test.indexOf('cub100') > 0){
        $footer.html('<p>Copyright © 2018 '+corporationList[7].name+' All Rights Reserved <br>'+corporationList[7].num+'</p>')
    }else if(test.indexOf('ztkao') > 0){
        $footer.html('<p>Copyright © 2018 '+corporationList[8].name+' All Rights Reserved <br>'+corporationList[8].num+'</p>')
    }else if(test.indexOf('qcwedu') > 0){
        $footer.html('<p>Copyright © 2018 '+corporationList[9].name+' All Rights Reserved <br>'+corporationList[9].num+'</p>')
    }else if(test.indexOf('yytvb') > 0){
        $footer.html('<p>Copyright © 2018 '+corporationList[10].name+' All Rights Reserved <br>'+corporationList[10].num+'</p>')
    }else if(test.indexOf('591book') > 0){
        $footer.html('<p>Copyright © 2018 '+corporationList[11].name+' All Rights Reserved <br>'+corporationList[11].num+'</p>')
    }else if(test.indexOf('kangerwang') > 0){
        $footer.html('<p>Copyright © 2018 '+corporationList[12].name+' All Rights Reserved <br>'+corporationList[12].num+'</p>')
    }else if(test.indexOf('ytkj') > 0){
        $footer.html('<p>Copyright © 2018 '+corporationList[13].name+' All Rights Reserved <br>'+corporationList[13].num+'</p>')
     }
})
</script>
```
## html5shiv
```
<!--if lt IE 9]>　　
    <script src="https://cdn.bootcss.com/html5shiv/r29/html5.js"></script>　　
<![endif]-->
```
## m端手指滑动事件
```
<script>
    //返回角度
    function GetSlideAngle(dx, dy) {
        return Math.atan2(dy, dx) * 180 / Math.PI;
    }

    //根据起点和终点返回方向 1：向上，2：向下，3：向左，4：向右,0：未滑动
    function GetSlideDirection(startX, startY, endX, endY) {
        var dy = startY - endY;
        var dx = endX - startX;
        var result = 0;

    //如果滑动距离太短
    if(Math.abs(dx) < 2 && Math.abs(dy) < 2) {
      return result;
    }

    var angle = GetSlideAngle(dx, dy);
    if(angle >= -45 && angle < 45) {
      result = 4;
    }else if (angle >= 45 && angle < 135) {
      result = 1;
    }else if (angle >= -135 && angle < -45) {
      result = 2;
    }
    else if ((angle >= 135 && angle <= 180) || (angle >= -180 && angle < -135)) {
      result = 3;
    }
    return result;
    }

    //滑动处理
    var startX, startY;
    document.addEventListener('touchstart',function (ev) {
        startX = ev.touches[0].pageX;
        startY = ev.touches[0].pageY;
    }, false);
    document.addEventListener('touchend',function (ev) {
        var endX, endY;
        endX = ev.changedTouches[0].pageX;
        endY = ev.changedTouches[0].pageY;
        var direction = GetSlideDirection(startX, startY, endX, endY);
        switch(direction) {
            case 0:
                alert("没滑动");
                break;
            case 1:
                alert("向上");
                break;
            case 2:
                alert("向下");
                break;
            case 3:
                alert("向左");
                alert("!");
                break;
            case 4:
                alert("向右");
                break;
            default:
        }
    }, false);
</script>
```
## 复制微信

### 【html】
```
<!--弹出层 开始-->
<div class="weChatB w_2">
    <div class="title">加微信领取</div>
    <p class="weChatTitle yii_template">长按复制下方微信添加为好友<br>↓↓↓</p>
    <p class="weChatCenter wxnumber">
    </p>
    <p class="weChatBottom">微信咨询  免费获取信息</p>
</div>
<!--弹出层 结束-->

<div class="footerBar">
    <p>教师资格考试微信：<span class="c-yellow wxCode"></span>（点击复制）</p>
</div>
<div class="footH" style="height: 1.2rem"></div>
```
### 【css】
```
// 底部浮动条
.footerBar {
	width: 10rem;
	position: fixed;
	height: 1.2rem;
	bottom: 0;
	left: 50%;
	margin-left: -5rem;
	background-color: #E9360F;
}
.footerBar p {
	line-height: 1.2rem;
	font-size: 0.4rem;
	color: #fff;
	text-align: center;
}
.footerBar .c-yellow {
	color: #FFF83A;
}
// 微信弹窗
.weChatB {
	display: none;
	width: 8.36rem;
	height: 6.066666666666666rem;
	background: rgba(0,0,0,.1) url(../images/layer-wx.png) no-repeat center;
	background-size: cover;
}
.weChatB .title {
	height: 1.2533333333333334rem;
	font-size: 0.56rem;
	line-height: 1.2533333333333334rem;
	color: #FFFFFF;
	text-align: center;
}
.weChatTitle {
	text-align: center;
	margin: 0.7066666666666667rem auto 0.16rem ;
	font-size: 0.4rem;
	line-height: 0.6666666666666666rem;
	color: #ff452d;
}
.weChatCenter {
	width: 5.04rem;
	height: 1.24rem;
	display: block;
	font-weight: bold;
	background: #ff1a1f;
	border-radius: 0.49333333333333335rem;
	margin: 0 auto;
	font-size: 0.56rem;
	color: #FFFFFF;
	text-align: center;
	line-height: 1.2933333333333332rem;
}
.weChatBottom {
	text-align: center;
	font-weight: bold;
	font-size: 0.5rem;
	line-height: 0.5333333333333333rem;
	color: #ff1a1f;
	margin-top: 0.3466666666666667rem;
}
```
### 【js】
```
<script src="js/clipboard.min.js"></script>

// --------------微信修改处-------------

    var wxNums = ['qbk1303','qbk1253'];
    var count = Math.floor(Math.random()*wxNums.length);
    var wxNow = wxNums[count];
    $('.wxnumber'). html(wxNow);
    $('.wxCode'). html(wxNow);

    $(document).on("click", ".xnkf", function () {
        layer.open({
            type: 1,
            title: false,
            content: $('.w_2'),
            closeBtn: 0,
            shadeClose: true,
            shade: [0.7, '#000'],
            anim: 2
        })
    });

// --------------复制微信--------------
    var clipboard = new Clipboard('.wxCode');
    $('.wxCode').on('click', function() {
        $('.wxCode').attr('data-clipboard-text', wxNow);
    });
    clipboard.on('success', function(e) {
        layer.msg('复制成功')
    });
    clipboard.on('error', function(e) {
    $(document).on("click", ".xnkf", function () {
        layer.open({
            type: 1,
            title: false,
            content: $('.w_2'),
            closeBtn: 0,
            shadeClose: true,
            shade: [0.7, '#000'],
            anim: 2
        })
    });
        layer.msg('当前浏览器不支持点击复制，请长按复制')
    });

    var clipboard2 = new Clipboard('.wxnumber');
    $('.wxnumber').on('click', function() {
        $('.wxnumber').attr('data-clipboard-text', wxNow);
    });
    clipboard2.on('success', function(e) {
        layer.msg('复制成功')
    });
    clipboard2.on('error', function(e) {
        layer.msg('当前浏览器不支持点击复制，请长按复制')
    });
```
## 轮播图
### 【html】
```
<div class="w" id="slide2">
    <div class="content" >
        <ol class="control clearfix">
            <li data-i="0" class="active">精炼预测班</li>
            <li data-i="1">速升实战班</li>
            <li data-i="2">面试通关班</li>
            <li data-i="3">密训保过班</li>
        </ol>
        <ul class="slider">
            <li><img src="images/427-slide1.jpg" alt="1"><button class="xnkf btn-3"><i class="ico-talk"></i>立即咨询</button></li>
            <li><img src="images/427-slide2.jpg" alt="2"><button class="xnkf btn-3"><i class="ico-talk"></i>立即咨询</button></li>
            <li><img src="images/427-slide3.jpg" alt="3"><button class="xnkf btn-3"><i class="ico-talk"></i>立即咨询</button></li>
            <li><img src="images/427-slide4.jpg" alt="4"><button class="xnkf btn-3"><i class="ico-talk"></i>立即咨询</button></li>
        </ul>

    </div>
    <div class="bar">
        <div class="l"><img src="images/427-ico-left.png" alt="l"></div>
        <div class="r"><img src="images/427-ico-right.png" alt="r"></div>
    </div>
</div>
```
### 【js】
```
// 轮播
function mySlide(id) {
    var $slide = $(id);
    var slide = document.querySelector(id);
    var speed = 666;  // 动画时间
    var easing = 'swing';  // 动画曲线
    var interval = 4000;  // 轮播切换时间
    var count = 0;
    var imgs = $slide.find('.slider>li');
    var conts = $slide.find(".control>li");
    var l = $slide.find(".l");
    var r = $slide.find(".r");
    var max = imgs.length - 1;
    var width = imgs[0].offsetWidth;

    function change(num) {
        if (num > count) {
            if (num > max) {
                num = 0;
            }
            $(imgs[num]).css('left', width * 2);
            $(imgs[count]).stop().animate({left: '0'}, speed, easing);
            $(imgs[num]).stop().animate({left: width}, speed, easing);
        } else {
            if (num < 0) {
                num = max;
            }
            $(imgs[num]).css('left', '0px');
            $(imgs[count]).stop().animate({left: width * 2}, speed, easing);
            $(imgs[num]).stop().animate({left: width}, speed, easing);
        }
        count = num;
        $(conts[count]).addClass('active').siblings().removeClass('active');
    }
    //  左右控制点击事件
    l.on('click', function () {
        change(count - 1);
    });
    r.on('click', function () {
        change(count + 1);
    });
    //  序号控制点击事件
    conts.on('click', function () {
        change($(this).data('i'));
    });
    var times = null;
    times = setInterval(function () {
        change(count + 1);
    }, interval);
    // 鼠标经过动画暂停
    $slide.on('mouseover','.bar ,.control,.slider', function () {
        clearInterval(times);
    });
    $slide.on('mouseout','.slider,.control,.bar', function () {
        clearInterval(times);
        times = setInterval(function () {
            change(count + 1);
        }, interval);
    });
}
mySlide('#slide1');
mySlide('#slide2');
```
### 【js M端带滑屏事件】
```
function mySlide(id) {
    var $slide = $(id);
    var slide = document.querySelector(id);
    var speed = 666;  // 动画时间
    var easing = 'swing';  // 动画曲线
    var interval = 4000;  // 轮播切换时间
    var count = 0;
    var imgs = $slide.find('.slider>li');
    var conts = $slide.find(".control>li");
    var l = $slide.find(".l");
    var r = $slide.find(".r");
    var max = imgs.length - 1;
    var width = imgs[0].offsetWidth;

    function change(num) {
        if (num > count) {
            if (num > max) {
                num = 0;
            }
            $(imgs[num]).css('left', width * 2);
            $(imgs[count]).stop().animate({left: '0'}, speed, easing);
            $(imgs[num]).stop().animate({left: width}, speed, easing);
        } else {
            if (num < 0) {
                num = max;
            }
            $(imgs[num]).css('left', '0px');
            $(imgs[count]).stop().animate({left: width * 2}, speed, easing);
            $(imgs[num]).stop().animate({left: width}, speed, easing);
        }
        count = num;
        $(conts[count]).addClass('active').siblings().removeClass('active');
    }
    //  左右控制点击事件
    l.on('click', function () {
        change(count - 1);
    });
    r.on('click', function () {
        change(count + 1);
    });
    // 滑动屏幕控制轮播

    var startX, startY;
    slide.addEventListener('touchstart',function (ev) {
        clearInterval(times);

        startX = ev.touches[0].pageX;
        startY = ev.touches[0].pageY;
    }, false);
    slide.addEventListener('touchend',function (ev) {

        clearInterval(times);
        times = setInterval(function () {
            change(count + 1);
        }, interval);

        var endX, endY;
        endX = ev.changedTouches[0].pageX;
        endY = ev.changedTouches[0].pageY;
        var direction = GetSlideDirection(startX, startY, endX, endY);
        switch(direction) {
            case 0:
                // alert("没滑动");
                break;
            case 1:
                // alert("向上");
                break;
            case 2:
                // alert("向下");
                break;
            case 3:
                // alert("向左");
                change(count + 1);
                break;
            case 4:
                // alert("向右");
                change(count - 1);
                break;
            default:
        }
    }, false);

    //  序号控制点击事件
    conts.on('click', function () {
        change($(this).data('i'));
    });
    var times = null;
    times = setInterval(function () {
        change(count + 1);
    }, interval);
    // 鼠标经过动画暂停
    $(id).on('mouseover','.bar ,.control,.slider', function () {
        clearInterval(times);
    });
    $(id).on('mouseout','.slider,.control,.bar', function () {
        clearInterval(times);
        times = setInterval(function () {
            change(count + 1);
        }, interval);
    });
}
mySlide('#slide');

// 手指滑动事件

//返回角度
function GetSlideAngle(dx, dy) {
    return Math.atan2(dy, dx) * 180 / Math.PI;
}

//根据起点和终点返回方向 1：向上，2：向下，3：向左，4：向右,0：未滑动
function GetSlideDirection(startX, startY, endX, endY) {
    var dy = startY - endY;
    var dx = endX - startX;
    var result = 0;

    //如果滑动距离太短
    if(Math.abs(dx) < 2 && Math.abs(dy) < 2) {
        return result;
    }

    var angle = GetSlideAngle(dx, dy);
    if(angle >= -45 && angle < 45) {
        result = 4;
    }else if (angle >= 45 && angle < 135) {
        result = 1;
    }else if (angle >= -135 && angle < -45) {
        result = 2;
    }
    else if ((angle >= 135 && angle <= 180) || (angle >= -180 && angle < -135)) {
        result = 3;
    }

    return result;
}
```
### nav滚动
```
<script src="js/scrollPage.js"></script>
// 滚屏
    $(".common-module").scrollPage();
```
## 单页微信修改
```
<script>
    $(function () {
        var weixinArray = [];
        var wxList = [{
            "wxCode": "gp21209",
            "channelName": "zonghe",
            "id": 15,
            "channelId": 13,
            "qrImg": "#",
            "channelCode": "xueke"
        }];
        if(wxList != null) {
            for(var i = 0; i < wxList.length; i++) {
                weixinArray.push(wxList[i].wxCode);
            }
        }
        $(function() {
            var randomNum = Math.floor(Math.random() * weixinArray.length);
            var wxObject = weixinArray[randomNum]; //随机取一个公众号对应关系
            if(
                $(".code").length > 0) {
                $(".code").attr("data-clipboard-text", wxObject);
                $(".code").html(wxObject) //设置公众号值
            }
        })
    });
</script>
```
## m端fastClick
```
<script src="http://js.ykclass.com/frame/fastClick/v1.0.0/fastClick.js"></script>
// 快速点击
FastClick.attach(document.body);
```
## 小能代码
```
var kf = 'kf_9540_1520933792603';
var NTKF_PARAM = {
    "siteid": "kf_9540" /*网站siteid*/ ,
    "settingid": kf /*代码ID*/ ,
    "uid": "" /*会员ID*/ ,
    "uname": "" /*会员名*/ ,
    "userlevel": "0" /*会员等级*/
};
$(document).on("click", ".ntkf", function() {
    NTKF.im_openInPageChat(kf);
});
```
## 视频播放模块
### 【js】
```
<script src="http://static.ykclass.com/frame/polyv/polyvplayer.min.js"></script>

//视频
	var uid = "336d8745b4";
	var vid = "5af4dd0127c62475750485dc988b22d2_5";
	var videoPlayer = null; //live：直播播放器  video：点播播放器
	/**
	 * 绑定页面事件函数
	 */
	/**
	 * 初始化播放器
	 */
	initVidoPlayer(vid);
	/**
	 * 初始化点播播放器
	 * @param vid：视频id
	 */
	function initVidoPlayer(vid) {
		videoPlayer = polyvObject('#player').videoPlayer({
			'width': '100%',
			'height': '100%',
			'vid': vid,
			flashParams: {
				'allowScriptAccess': 'always',
				'allowFullScreen': 'true',
				'quality': 'high',
				'bgcolor': '#ffffff',
				'wmode': 'transparent',
			},
			flashvars: {
				'autoplay': '1',
				'is_auto_replay': 'on',
				'ban_history_time': 'on',
				'setScreen': 'fill',
			}
		});
	};
```
## 手机验证码模块

### 【html】
```
<!--弹出层 开始-->
			<div class="layer-warp">
                <div class="layer">
                    <div class="title">恭喜您，提交成功！</div>
                    <div class="text">
                        您好，您的信息已提交成功，<span class="c-b">查询结果将于15分钟内以短信或电话的方式通知您，</span>请注意查收！
                    </div>
                    <div class="layer-close"></div>
                </div>
            </div>
<!--弹出层 结束-->
```
### 【css  M】
```
.layer-warp {
	position: fixed;
	left: 0px;
	top: 0px;
	right: 0px;
	bottom: 0px;
	display: block;
	text-align: center;
	background: rgba(0, 0, 0, 0.4);
	z-index: 9999999;
	.layer {
		position: absolute;
		top: 50%;
		left: 35%;
		transform: translate(-35%, -50%);
		.w(700);
		.h(700);
		background: url(../images/layer.png) no-repeat;
		background-size: cover;
		z-index: 99999999;
	}
	.title {
		position: absolute;
		top: 110/75rem;
		left: 164/75rem;
		.fs(50);
		color: #fff;
	}
	.text {
		position: absolute;
		top: 260/75rem;
		left: 130/75rem;
		color: #666666;
		.w(490);
		.h(250);
		.fs(36);
		line-height: 1.5;
		text-align: left;
		.c-b {
			font-weight: bold;
			color: #333333;
		}
	}
	.layer-close {
		position: absolute;
		top: 514/@r;
		left: 125/@r;
		.w(485);
		.h(100);
	}
}
```
### 【css  PC】
```
/*弹窗部分开始*/
.layer-warp {
  position: fixed;
  left: 0px;
  top: 0px;
  right: 0px;
  bottom: 0px;
  display: none;
  text-align: center;
  background: rgba(0, 0, 0, 0.6);
  z-index: 9999999;
}
.layer-warp .layer {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 493px;
  height: 501px;
  background: url(../images/layer.png) no-repeat;
  background-size: cover;
  z-index: 99999999;
}
.layer-warp .text {
  margin-top: 190px;
  margin-left: 104px;
  color: #666666;
  height: 300px;
  width: 324px;
  font-size: 25px;
  line-height: 1.4;
  text-align: left;
}
.layer-warp .text .c-b {
  font-weight: bold;
  color: #333333;
}
.layer-warp .layer-close {
  position: absolute;
  top: 4.8rem;
  left: 1.2rem;
  z-index: 999999999;
  width: 4.66666667rem;
  height: 1.06666667rem;
}
/*弹窗部分结束*/
```
### 【html】
```
<article class="part-phone">
    <img src="images/phone.jpg" alt="免费预约">
    <div class="getPhone">
        <div class="phone">
            <input id="phone" class="phone-num" type="text" placeholder="请输入您的手机号码">
            <input type="button" class="send-phone" id="sendCode" value="获取动态码">
        </div>
        <div class="dt-num">
            <input type="text" id="codeValue"  placeholder="请输入动态码">
        </div>
        <button id="vailCode">
            查询结果  →
        </button>
    </div>
</article>
```
### 【js】
```
$('.layer-close').on('click',function () {
    $('.layer-warp').hide();
});

$("#phone").keyup(function() {
    var phone = $("#phone").val();
    if(phone.length > 11) {
        layer.msg('手机号超出字符限制！')
    }
});

$(function() {
    var countdown = 90;
    var nowHost = '';
    var nowProtocol = window.location.protocol;
    // 场景代码
    var cjCode = 'YK_M_GAOKUAI';
    if(nowProtocol == 'http:'){
        nowHost = "http://tf.topksw.com"
    }else {
        nowHost = "https://m.ykclass.com"
    }

    var settime = function(obj) {
        if(countdown == 0) {
            obj.removeAttr("disabled");
            obj.val("获取动态码");
            countdown = 60;
            return;
        } else {
            obj.attr("disabled", true);
            obj.val("重新发送(" + countdown + ")");
            countdown--;
        }
        setTimeout(function() {
            settime(obj);
        }, 1000)
    }

    var activity = {
        domainHost: nowHost,
        sendSms: function(phone, platform, callback) {
            var _this = this;
            var regPhone = /^0?1[3|4|5|7|8][0-9]\d{8}$/;
            if(!regPhone.test(phone)) {
                layer.msg('手机号码输入有误！')
            } else {
                settime($("#sendCode"));
                $.ajax({
                    type: "get",
                    url: _this.domainHost + "/common/sendSmsMessage.html",
                    dataType: "jsonp",
                    jsonp: "callback", //传递给请求处理程序或页面的，用以获得jsonp回调函数名的参数名(一般默认为:callback)
                    jsonpCallback: "callback", //自定义的jsonp回调函数名称，默认为jQuery自动生成的随机函数名，也可以写"?"，jQuery会自动为你处理数据
                    data: {
                        phone: phone,
                        platform: platform
                    },
                    success: function(data) {
                        if(callback && typeof callback == 'function') {
                            callback(data);
                        }
                    }
                })
            }
        }
        ,
        saveActivitySmsInfo: function(object, code, callback) {
            var _this = this;
            object.accessUrl = window.location.href;
            if(!code) {

            }
            object.code = code;
            console.log(object)
            $.ajax({
                type: "get",
                url: _this.domainHost + "/common/saveActivitySmsInfo.html",
                dataType: "jsonp",
                jsonp: "callback", //传递给请求处理程序或页面的，用以获得jsonp回调函数名的参数名(一般默认为:callback)
                jsonpCallback: "callback", //自定义的jsonp回调函数名称，默认为jQuery自动生成的随机函数名，也可以写"?"，jQuery会自动为你处理数据
                data: object,
                success: function(msg) {
                    if(callback && typeof callback == 'function') {
                        callback(msg);
                    }
                },
                error: function(data) {}
            })
        }
    };
    $("#sendCode").click(function() {
        activity.sendSms($("#phone").val(), "yk", function(msg) {
            if(msg.c == 100) {
                console.log(msg)
            }
        })
    });
    $("#vailCode").click(function() {

        var object = {
            sceneCode: cjCode,
            phone: $("#phone").val(),
            content: ''
        }
        var code = $("#codeValue").val();
        activity.saveActivitySmsInfo(object, code, function(msg) {
            if(msg.c == 100) {
                $(".layer-warp").show();
                $("input").not("#sendCode").val("");
            } else if(msg.m == '用户手机号不能为空') {
                layer.msg('手机号码不能为空');
            } else if(msg.m == '短信验证码不能为空!') {
                layer.msg('短信验证码不能为空!');
            } else if(msg.code == 202) {
                layer.msg('短信验证码错误!');
            } else {
                layer.msg('您的信息输入有误');
            }

        })
    })
```
### 【js--无短信验证】
```
$("#phone").keyup(function() {
    var regPhone = /^0?1[3|4|5|7|8][0-9]\d{8}$/;
    var phone = $("#phone").val();
    if(phone.length > 11) {
        layer.msg('手机号超出字符限制！')
    }
});
$(function() {
    var nowHost = '';
    var nowProtocol = window.location.protocol;
    // 场景代码
    var cjCode = 'YK_M_GAOKUAI';
    if(nowProtocol == 'http:'){
        nowHost = "http://tf.topksw.com"
    }else {
        nowHost = "https://m.ykclass.com"
    }
    var activity = {
        domainHost: nowHost,

        saveActivitySmsInfo: function(object, code, callback) {
            var _this = this;
            object.accessUrl = window.location.href;
            var regPhone = /^0?1[3|4|5|7|8][0-9]\d{8}$/;
            if(!regPhone.test(object.phone)) {
                layer.msg('手机号码输入有误！')
            } else {
                object.code = code;
                console.log(object);
                $.ajax({
                    type: "get",
                    url: _this.domainHost + "/common/saveActivityInfo.html",
                    dataType: "jsonp",
                    jsonp: "callback", //传递给请求处理程序或页面的，用以获得jsonp回调函数名的参数名(一般默认为:callback)
                    jsonpCallback: "callback", //自定义的jsonp回调函数名称，默认为jQuery自动生成的随机函数名，也可以写"?"，jQuery会自动为你处理数据
                    data: object,
                    success: function (msg) {
                        if (callback && typeof callback == 'function') {
                            /**
                             **    msg.c : 100 保存成功
                             msg.c : 200:保存失败
                             msg.c : 202 短信验证码错误
                             msg.m   错误消息
                             **
                             **/
                            callback(msg);
                        }
                    },
                    error: function (data) {
                    }
                })
            }
        }
    };

    $("#vailCode").click(function() {
        var Province = $('.province').text();
        var object = {
            sceneCode: cjCode,
            phone: $("#phone").val(),
            content: Province
        };
        var code = $("#codeValue").val();
        activity.saveActivitySmsInfo(object, code, function(msg) {
            if(msg.c == 100) {
                layer.msg('查询成功！系统将以电话形式通知您结果。');
            } else if(msg.m == '用户手机号不能为空') {
                layer.msg('手机号码不能为空');
            } else if(msg.m == '短信验证码不能为空!') {
                layer.msg('短信验证码不能为空!');
            } else if(msg.code == 202) {
                layer.msg('短信验证码错误!');
            } else {
                layer.msg('您的信息输入有误');
            }
        })
    })
});
```
## 倒计时模块
```
var today = new Date().getTime();
var  examDay = [2018,4,24];
var endDay = new Date(examDay[0], examDay[1]-1, examDay[2]).getTime();
if(endDay - today > 0) {
    var day = Math.ceil((endDay - today) / (24 * 60 * 60 * 1000));
    var single = day % 10;
    var decade = parseInt((day % 100) / 10);
    var hundreds = parseInt((day % 1000) / 100);
    $(".single").html(single);
    $(".decade").html(decade);
}
```