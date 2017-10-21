# MybatisReverseProject
mybatis逆向工程
     
1.使用的mybatis-generator-core是借鉴githup上的一个兄弟改写源码的，他的已经能满足我的需求了有需要的同学可以自己去改写：
  改写的内容如下：
	1.生成的*mapper.xml文件中使用4个空格来缩进     
	2.生成的*mapper.xml文件中每个元素间增加一空行，如insert,update,delete等之间增加一空行      
	3.去掉*mapper.xml文件中生成的注释      
	4.根据数据库表名及字段的注释为Java类、属性增加注释，可以在源码org.mybatis.generator.internal.db.DatabaseIntrospector.java类中根据个人情况进行修改    
	5.实现每次生成都覆盖生成文件 
	
2.使用方法
   2.1 首先在/MybatisReverseProject/config/generatorConfig.xml文件中配置数据库连接的信息
   2.2其次配置生成实体类的位置、生成mapper映射文件生成的位置、生成mapper接口生成的位置，以上配置的3个路径为你项目的路径；指定要逆向生成代码的数据库的表
   
   2.3 启动主程序GeneratorSqlmap.java
    
