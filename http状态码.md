## 我遇见的HTTP状态码

> 一. 502 Bad Gateway
    
     出现原因：对用户访问请求的响应超时造成的
     
     解决：
      1.提高 Web 服务器的响应速度，也即减少内部的调用关系，可以把需要的页面、素材或数据，缓存在内存中，可以是专门的缓存服务器，
      也可以Web服务器自身的缓存，提高响应速度；
      2.网络带宽的问题，则对传输的数据包进行压缩处理，或者向IDC申请增加带宽；
      3.属于内部网络的故障或设置问题，也即内部网络拥塞，可能内部存在大量的数据调用或交互造成的，则需要优化内部网络传输或协议；
      4.数据库的数据读取造成前端服务器 ，响应用户的请求变慢，那么必须提高数据库的处理能力，
      若是只读业务可以增加数据缓存的模式 或者增加数据库备机，分散读压力； 
      若是写的压力，则可以考虑延迟写的模式，想这个时候做数据写分散肯定来不及
