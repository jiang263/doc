
# uc-qq-share-to-wechat

github: https://github.com/AngusFu/uc-qq-share-to-wechat


触发手机 UC/QQ 浏览器的原生的微信分享功能



## 安装

```
	npm install --save ucshare

```

## 使用

```
	var mShare = require('ucshare');

	/**
	 * @param  {Object} config 配置对象  参数见示例
	 * config = {
	 *      title : 'Lorem ipsum dolor sit.',
	 *      url   : 'http://m.ly.com',
	 *      desc  : 'Lorem ipsum dolor sit.',
	 *      img   : 'http://img1.40017.cn/cn/s/c/2015/loading.gif',
	 *      type  : type // 1 ==> 朋友圈  2 ==> 朋友  0 ==> 直接弹出原生
	 * };
	 */
	var mshare = new mShare({
	      title : 'Lorem ipsum dolor sit.',
	      url   : 'http://m.ly.com',
	      desc  : 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quaerat inventore minima voluptates.',
	      img   : 'http://placehold.it/150x150'
	});

	$('button').click(function () {
	    // 1 ==> 朋友圈  2 ==> 朋友  0 ==> 直接弹出原生
	    mshare.init(+$(this).data('mshare'));
	});



```

### 说明

此插件主要作用是在UC和QQ两个手机浏览器上面触发微信分享到朋友圈或发送给朋友的功能

