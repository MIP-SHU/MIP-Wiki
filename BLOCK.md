## MIP-Block wiki

### 登录状态
  ```key``` : token+"Login"    
  ```value``` : 0（_未登录_） 1（_已登录_）
  
### 访问次数（*设置60秒过期时间*）
  ```key``` : token  
  ```value``` : count（*访问次数*）
  
### LOG 表
##### IP集合
  ```key``` : IpSet  
  ```value``` ：remoteIP（*访问过的IP值*）
##### IP对应的访问Log
  ```key``` : remoteIp+"Collections"  
  ```value``` : expression-time-token （*依次对应检索内容-检索时间-当前IP对应的token，中间以"-"间隔*）  
##### Ip 对应的访问次数
  ```key```: Ip+"CountIp"  
  ```value``` : count（*Ip访问次数*）
