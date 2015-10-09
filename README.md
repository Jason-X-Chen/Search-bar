# Search-bar
智能搜索框
调试工具和库：Fiddler,jQuery<br>
搜索框功能：智能提示<br>
使用技术：借助jQuery脚本完成动态渲染；事件绑定和事件代理；<br>

上一版本借助fiddler反向代理的方法实现Ajax通信<br>
新版本改为采用JSONP实现跨区请求百度搜索的API<br>
以下描述的是上一版本的方法，缺点在于不能直接使用，每次使用要开fiddler<br>
实现下拉框智能提示功能，使用了Bing搜索的API,其他搜索引擎自动提示API也是一样的<br>
调试步骤：<br>
首先，使用Fiddler的Composer模拟Ajax请求，确定请求可以成功<br>
例如：GET http://bj1.api.bing.com/qsonhs.aspx?q=d 查看返回的json数据的结构<br>
接着，因为Ajax请求的同源策略，使用fiddler的AutoResponder将bj1.api.bing.com/域名下的文件替换成相应的本地文件<br>
