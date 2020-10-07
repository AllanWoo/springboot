## 佛丁丁-Oracle

本仓库为[佛丁丁](https://github.com/AllanWoo/springboot.git)的oracle版本 `(保持同步更新)` 

如需单应用版本请切换[fast分支](https://github.com/AllanWoo/springboot.git)

初始密码：用户名 admin 密码123456

她可以用于所有的Web应用程序，如网站管理后台，网站会员中心，CMS，CRM，OA。所有前端后台代码封装过后十分精简易上手，出错概率低。

## 内置功能
1.  用户管理：用户是系统操作者，该功能主要完成系统用户配置。
2.  部门管理：配置系统组织机构（公司、部门、小组），树结构展现支持数据权限。
3.  岗位管理：配置系统用户所属担任职务。
4.  菜单管理：配置系统菜单，操作权限，按钮权限标识等。
5.  角色管理：角色菜单权限分配、设置角色按机构进行数据范围权限划分。
6.  字典管理：对系统中经常使用的一些较为固定的数据进行维护。
7.  参数管理：对系统动态配置常用参数。
8.  通知公告：系统通知公告信息发布维护。
9.  操作日志：系统正常操作日志记录和查询；系统异常信息日志记录和查询。
10. 登录日志：系统登录日志记录查询包含登录异常。
11. 在线用户：当前系统中活跃用户状态监控。
12. 定时任务：在线（添加、修改、删除)任务调度包含执行结果日志。
13. 代码生成：前后端代码的生成（java、html、xml、sql）支持CRUD下载 。
14. 系统接口：根据业务代码自动生成相关的api接口文档。
15. 服务监控：监视当前系统CPU、内存、磁盘、堆栈等相关信息。
16. 在线构建器：拖动表单元素生成相应的HTML代码。
17. 连接池监视：监视当前系统数据库连接池状态，可进行分析SQL找出系统性能瓶颈。

## 如何使用

#### 1、准备工作
~~~
jdk>=1.8 (推荐1.8)
oracle>=10g (推荐使用11g)
maven>=3.0
开发工具：idea 或者 eclipse
~~~

#### 2、下载代码
下载地址： https://github.com/AllanWoo/springboot.git

推荐使用git clone下载，有效进行代码更新

#### 3、数据库

使用dba权限的用户连接数据库,创建数据库
```sql
create user ry identified by ry;
grant connect, resource to ry;
```
导入项目sql文件夹里的sql脚本：`ry_yyyymmdd(更新日期).sql` 和 `quartz.sql`

#### 4、配置修改

编辑resources目录下的application-druid.yml，修改数据库连接

```yml
url: 服务器地址
username: 账号
password: 密码
```

编辑resources目录下的application.yml，修改开发环境配置
```yml
port: 端口
context-path: 部署路径
```

#### 5、启动项目
执行文件`RuoYi-Oracle/ruoyi-admin/src/main/java/com/ruoyi/RuoYiApplication.java`的main函数即可。

## 文档
[佛丁丁官方文档](http://doc.ruoyi.vip) http://doc.ruoyi.vip

## 演示图

<table>
    <tr>
        <td><img src="http://goddesslzj.xyz/foding.png"/></td>
        <td><img src="http://goddesslzj.xyz/img/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_202010071406261.png"/></td>
    </tr>
    <tr>
        <td><img src="http://goddesslzj.xyz/img/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_202010071406262.png"/></td>
        <td><img src="http://goddesslzj.xyz/img/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_202010071406263.png"/></td>
    </tr>
    <tr>
        <td><img src="http://goddesslzj.xyz/img/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_202010071406264.png"/></td>
        <td><img src="http://goddesslzj.xyz/img/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_202010071406265.png"/></td>
    </tr>
	
</table>

## 请作者喝杯咖啡
<div>
<img src="http://img.racinfo.cn/007FMAUigy1g68fpr0s1lj30g40g4q58.jpg" width="350" height="350">
<img src="http://img.racinfo.cn/007FMAUigy1g68focark1j30g40g4wfe1.jpg" width="350" height="350">
</div>
