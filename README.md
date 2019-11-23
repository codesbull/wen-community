## 章鱼社区

### [在线地址](http://www.zykcoderman.xyz)  

## 技术栈
1. SpringBoot。Thymeleaf模板引擎。
2. 数据访问层：Mybatis。
3. 数据库：MySql。
4. 服务器：内置Tomcat。
5. 前端相关:Jquery,Bootstrap，Ajax，Layer等。
6. 文件上传：OSS对象存储。
7. 短信验证：阿里云的短信服务。
8. 富文本编辑器：Editormd。
9. OAuth2授权登入（Github , 百度，QQ）
10. Redis分布式内存数据库，实现热点数据缓存，每日签到。

## 快速运行
1. 安装必备工具  
JDK，Maven, Redis，git
2. 克隆代码到本地  

3. 运行命令创建数据库脚本

4. 运行打包命令
```sh
mvn package
```
5. 运行项目  
```sh
java -jar target/coderman-0.0.1-SNAPSHOT.jar
```
## 目录结构

主要目录结构如下：

~~~
├─coderman              应用目录
│  ├─controller         控制器目录
│  ├─modal              映射数据库实体类
│  ├─dto                网络传输对象
│  ├─intercepter        拦截器
│  ├─myenums            枚举类
│  ├─provider           提供者
│  ├─service            业务逻辑层
│  ├─advice             配置类
│  ├─exception          自定义异常
│  ├─dao                数据访问层
│  ├─utils              工具类
│  ├─test               测试类
~~~~

6. 访问项目
```
http://localhost:8080
```
## 主要功能
1. 发帖
2. 选择分类
3. 选择标签
4. 评论
5. 通知
6. 关注
7. 点赞
8. 登入，注册
9. 搜索
10. 话题
12. 排序
13. 聊天室
14. 签到

## 部署
1. 阿里云ESC云主机部署

## 资料
[Spring 文档](https://spring.io/guides)    
[Spring Web](https://spring.io/guides/gs/serving-web-content/)   
[es](https://elasticsearch.cn/explore)    
[Github deploy key](https://developer.github.com/v3/guides/managing-deploy-keys/#deploy-keys)    
[Bootstrap](https://v3.bootcss.com/getting-started/)    
[Github OAuth](https://developer.github.com/apps/building-oauth-apps/creating-an-oauth-app/)    
[Spring](https://docs.spring.io/spring-boot/docs/2.0.0.RC1/reference/htmlsingle/#boot-features-embedded-database-support)    
[菜鸟教程](https://www.runoob.com/mysql/mysql-insert-query.html)    
[Thymeleaf](https://www.thymeleaf.org/doc/tutorials/3.0/usingthymeleaf.html#setting-attribute-values)    
[Spring Dev Tool](https://docs.spring.io/spring-boot/docs/2.0.0.RC1/reference/htmlsingle/#using-boot-devtools)  
[Spring MVC](https://docs.spring.io/spring/docs/5.0.3.RELEASE/spring-framework-reference/web.html#mvc-handlermapping-interceptor)  
[Markdown 插件](http://editor.md.ipandao.com/)   
[UFfile SDK](https://github.com/ucloud/ufile-sdk-java)  
[Count(*) VS Count(1)](https://mp.weixin.qq.com/s/Rwpke4BHu7Fz7KOpE2d3Lw)  

## 工具
[Git](https://git-scm.com/download)   
[Visual Paradigm](https://www.visual-paradigm.com)    
[Flyway](https://flywaydb.org/getstarted/firststeps/maven)  
[Lombok](https://www.projectlombok.org)    
[ctotree](https://www.octotree.io/)   
[Table of content sidebar](https://chrome.google.com/webstore/detail/table-of-contents-sidebar/ohohkfheangmbedkgechjkmbepeikkej)    
[One Tab](https://chrome.google.com/webstore/detail/chphlpgkkbolifaimnlloiipkdnihall)    
[Live Reload](https://chrome.google.com/webstore/detail/livereload/jnihajbhpnppcggbcgedagnkighmdlei/related)  
[Postman](https://chrome.google.com/webstore/detail/coohjcphdfgbiolnekdpbcijmhambjff)

## 脚本
```sql
CREATE TABLE USER
(
    ID int AUTO_INCREMENT PRIMARY KEY NOT NULL,
    ACCOUNT_ID VARCHAR(100),
    NAME VARCHAR(50),
    TOKEN VARCHAR(36),
    GMT_CREATE BIGINT,
    GMT_MODIFIED BIGINT
);
```
## 更新
1. 2019.10.21:添加积分模块，实现每日点赞
2. 每日签到可获得10积分
3. 2019.10.22：当你的问题被别人收藏的时候可以获得5点积分.
3. 当你的问题被别人点赞的时候你可以获得2积分

## 联系
章鱼社区交流群:830790908

