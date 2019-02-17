js对文字进行编码涉及3个函数：escape,encodeURI,encodeURIComponent，相应3个解码函数：unescape,decodeURI,decodeURIComponent
1、传递参数时需要使用encodeURIComponent，这样组合的url才不会被#等特殊字符截断。
        例如：<a href="http://passport.baidu.com/?logout&aid=7&u= +encodeURIComponent("http://cang.baidu.com/bruce42"
2. 进行url跳转时可以整体使用encodeURI。
        Location.href=encodeURI("http://cang.baidu.com/do/s?word=百度&ct=21");
3、js使用数据时可以使用escape 
        例如：搜藏中history纪录
