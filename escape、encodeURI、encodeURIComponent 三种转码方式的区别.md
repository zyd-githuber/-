## js对文字进行编码涉及3个函数：
 ### 1. escape 
    用途: js使用数据时可以使用escape  
    例如：搜藏中history纪录
 ### 2. encodeURI  
    用途：进行url跳转时可以整体使用encodeURI。  
    例如：Location.href=encodeURI("http://cang.baidu.com/do/s?word=百度&ct=21");
 ### 3. encodeURIComponent
    用途：传递参数时需要使用encodeURIComponent，这样组合的url才不会被#等特殊字符截断。
    例如：<a href="http://passport.baidu.com/?logout&aid=7&u= +encodeURIComponent("http://cang.baidu.com/bruce42"）
   
## 相应3个解码函数：
 - unescape
 - decodeURI
 - decodeURIComponent
