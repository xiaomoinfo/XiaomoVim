#项目启动步骤

1： 使用 本文件夹中的 sql文件创建数据库与数据库表

2: 修改 resources/db_config.properties 文件，填入正确的数据库连接用户名、密码

3: 打开 com.xiaomo.timeMachine包下的 timeMachineConfig 文件并运行

4: 打开浏览器输入  localhost 即可查看运行效果

注意： 请确保您安装了 JavaSE 1.6 或更高版本，tomcat下运行项目需要先删除 jetty-server-xxx.jar，否则会有冲突
maven 中用 provided 过滤 依赖


#gitignore不生效的原因和解决办法

无效的原因是：对应的目录或者文件已经被git跟踪，此时再加入.gitignore后就无效了，

解决办法：
执行 git rm -r --cached .idea 删掉git己经管理的idea文件

