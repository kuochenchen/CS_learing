# MAVEN
## MAVEN简介
 -为什么这么小？因为没有jar包
### 小结
  - MAVEN的好处
  - 一键构建：编译 测试（junit） 运行 打包
   * 依赖管理 对jar包的统一管理 节省空间 一件构建 可以跨平台  应用于大型项目 
   * 传统项目 按照业务分
   * 传统项目 按层分:Entity DAO Service 
## 项目构建
 mvn compile
 mvn test
 mvn package 打包
 mvn install 项目发布到本地仓库
 maven生命周期
  三种 
    clean
    defualt
    site
 执行顺序 compile test package install depoly
## 项目构建
  1. 跳过骨架选择 因为选择了骨架之后创建的web项目的目录不全 没有resource目录（存配置文件），还得手动创建
  2. 输入坐标 输入公司或组织名称 输入项目或模块名称
  3. 处理红色叉号
  4. 处理编译版本
  5. 创建Servlet
  6. 修改web.xml,删除多余的命名空间
  7. 打开maven仓库的视图
  8. maven运行 添加jar包的时候要选择依赖范围：
  - Compile  
  - Provided 编译时需要，测试时也需要，运行时不需要，打包时也不需要 
  - Runtime 数据库驱动包，编译时不需要，
  - Test 编译时不需要，测试时需要，运行时不需要 
### 小结：
  - 坐标
  - package
  -  
  
## 解决版本冲突
 - 就近者原则
 - 第一声明者原则
 - 排除原则
 - 版本锁定 
 
 
# 分模块开发 、
创建付工程
发布到本地仓库
创建dao模块
发布到本地仓库
创建service模块
发布到本地仓库
创建Web模块

创建私服Nexus
