MBG逆向工程
mybatis框架必备：实体类  自定义mapper接口 mapper.xml
传统实现需手动实现
逆向工程可以自动创建以上三个组件。 只能运行一次 要重新运行需删掉之前创建的
如何使用：
Mybatis Generator 简称MBG   代码生成器  自带基本CURD操作
依赖
        <dependency>
            <groupId>org.mybatis</groupId>
            <artifactId>mybatis</artifactId>
            <version>3.5.5</version>
        </dependency>
        <dependency>
            <groupId>mysql</groupId>
            <artifactId>mysql-connector-java</artifactId>
            <version>8.0.21</version>
        </dependency>
        <!--MBG-->
        <dependency>
            <groupId>org.mybatis.generator</groupId>
            <artifactId>mybatis-generator-core</artifactId>
            <version>1.3.2</version>
        </dependency>
MBG配置文件
1 JDBCConnection配置数据库连接信息
2 javaModelGenerator配置JAVABEAN的生成策略
3 sqlMapGenerator配置sql映射生成策略
4 javaClientGenerator配置Mapper接口的生成策略
5 table配置目标数据库（tableName:表名，domainObjectName:JavaBean类名）

配置完 运行test
