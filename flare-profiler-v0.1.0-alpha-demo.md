### Flare Profiler v0.1.0-alpha demo

到目前为止，Flare Profiler实现了对JVM取样分析功能，还不是很完善，欢迎大家测试使用，有任何问题请及时反馈给我。  
Flare Profiler 使用Rust语言编写，支持Windows、Linux、macOS系统，目前只调用JVM接口，不依赖系统API。  
主要包含以下三个部分：   
flare-agent： 注入到JVM执行的JVMTI模块  
flare-server：  采样数据收集及分析服务  
flare-ui:   Web实现的交互操作界面  
  
下面是几张截图及一个演示的例子。  
一个演示片段  
![GitHub](https://github.com/kylixs/kylixs.github.io/blob/master/flare-profiler/images/v0.1.0/demo-1.gif?raw=true)  
   
Profile（会话及历史）  
![GitHub](https://github.com/kylixs/kylixs.github.io/blob/master/flare-profiler/images/v0.1.0/profile.png?raw=true)  
  
Dashboard（概要信息）  
![GitHub](https://github.com/kylixs/kylixs.github.io/blob/master/flare-profiler/images/v0.1.0/dashboard.png?raw=true)  
  
Threads（线程CPU时间）  
![GitHub](https://github.com/kylixs/kylixs.github.io/blob/master/flare-profiler/images/v0.1.0/threads.png?raw=true)  

Call Graph （调用栈火焰图）  
![GitHub](https://github.com/kylixs/kylixs.github.io/blob/master/flare-profiler/images/v0.1.0/call_graph_1.png?raw=true)  
  
![GitHub](https://github.com/kylixs/kylixs.github.io/blob/master/flare-profiler/images/v0.1.0/call_graph_2.png?raw=true)  
  
![GitHub](https://github.com/kylixs/kylixs.github.io/blob/master/flare-profiler/images/v0.1.0/call_graph_3.png?raw=true)  
  
