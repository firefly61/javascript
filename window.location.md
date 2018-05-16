## window.location分析

* window.location
  
  window.location.href = 'url'
  
  window.location.relpace('url');
    
    *将地址替换成新url，该方法通过指定URL替换当前缓存在历史里（客户端）的项目，因此当使用replace方法之后，你不能通过“前进”和“后 退”来访问已经被替换的URL，这个特点对于做一些过渡页面非常有用！
  
  window.location.reload();
  
    *强制刷新页面，从服务器重新请求！
