# Search-bar
智能搜索框
调试工具和库：Fiddler,jQuery<br>
搜索框功能：智能提示<br>
使用技术：借助jQuery&JS脚本完成动态效果；事件绑定和事件代理；Ajax通信<br>

实现下拉框智能提示功能，使用了Bing搜索的API,其他搜索引擎自动提示API也是一样的<br>
调试步骤：<br>
首先，使用Fiddler的Composer模拟Ajax请求，确定请求可以成功<br>
例如：GET http://bj1.api.bing.com/qsonhs.aspx?q=d 查看返回的json数据的结构<br>
接着，因为Ajax请求的同源策略，使用fiddler的AutoResponder将bj1.api.bing.com/域名下的文件替换成相应的本地文件<br>
