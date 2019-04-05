# Spring 知识体系的总结
## Spring DI
## Spring AOP
  ### 定义AOP术语
  - 通知（advice）
  - 连接点（Join Point）
  - 切点（Point Cut）
  - 引入(introduction)
  - 织入（Weaving）
  **总结这几个术语之间的关系，通知包含了需要用于多个应用对象的横切行为；连接点是程序执行过程中能够应用通知的所有点；切点定义了通知被应用的具体位置（那些连接点。）其中最关键的概念是其诶单定义了那些连接点会得到通知**
  
  
  # Spring MVC知识体系
  ## 关键词
  - 处理映射器（Handle Mapper）
  - 控制器（Controller）
  - 视图解析器（View resolve）
  - DispatcherServlet 
  - ContextLoaderLisener
  - Spring 应用上下文
  - Web应用上下文
 ## 跟踪SpringMVC 请求
  ### 前景概要
  - Servlet3.0环境中，容器会自动在类路径下查找实现实现java.servlet.ServletContainerInitializer接口的类，如果发现有，那么就用它来配置Servlet容器
  - Spring提供了这个接口的实现，名字叫SpringServletContainerinitializer，这个类反过来又会查找实现WebApplicationinitializer的类并将配置任务交给它来完成
  - Spring3.2引入了一个便利的wenApplicationInitializer基础实现，也就是AbstractAnnotationConfigDispacherServletInitializer。
  ###  DispatcherServlet和ContextLoaderLisener之间的关系
  - DispatcherServlet加载包含Web组件的bean，入控制器，视图解析器，和处理映射
  - ContextLoaderLisene要加载应用中的其他bean,这些bean通常是驱动应用后端的中间层和数据层组件
  
  
  
