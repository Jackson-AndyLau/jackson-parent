# jackson-parent

## 父级依赖项目包

```HTML
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
  <modelVersion>4.0.0</modelVersion>
  <groupId>com.huazai</groupId>
  <artifactId>huazai-parent</artifactId>
  <version>0.0.1-SNAPSHOT</version>
  <packaging>pom</packaging>
  <!-- 集中定义依赖版本号 -->
	<properties>
		<junit.version>4.12</junit.version>
		<spring.version>4.2.4.RELEASE</spring.version>
		<mybatis.version>3.2.8</mybatis.version>
		<mybatis.spring.version>1.2.2</mybatis.spring.version>
		<mybatis.paginator.version>1.2.15</mybatis.paginator.version>
		<mysql.version>5.1.32</mysql.version>
		<slf4j.version>1.6.4</slf4j.version>
		<jackson.version>2.4.2</jackson.version>
		<druid.version>1.0.9</druid.version>
		<httpclient.version>4.5.10</httpclient.version>
		<jstl.version>1.2</jstl.version>
		<servlet-api.version>2.5</servlet-api.version>
		<jsp-api.version>2.0</jsp-api.version>
		<joda-time.version>2.5</joda-time.version>
		<commons-lang3.version>3.3.2</commons-lang3.version>
		<commons-io.version>1.3.2</commons-io.version>
		<commons-net.version>3.3</commons-net.version>
		<pagehelper.version>3.4.2-fix</pagehelper.version>
		<jsqlparser.version>0.9.1</jsqlparser.version>
		<commons-fileupload.version>1.3.1</commons-fileupload.version>
		<jedis.version>2.7.2</jedis.version>
		<solrj.version>4.10.3</solrj.version>
		<dubbo.version>2.5.3</dubbo.version>
		<zookeeper.version>3.4.7</zookeeper.version>
		<zkclient.version>0.1</zkclient.version>
		<activemq.version>5.13.0</activemq.version>
		<freemarker.version>2.3.28</freemarker.version>
		<quartz.version>2.2.2</quartz.version>
	</properties>
	<dependencies>
		<dependency>
			<groupId>junit</groupId>
			<artifactId>junit</artifactId>
			<scope>test</scope>
		</dependency>
	</dependencies>
	<dependencyManagement>
		<dependencies>
			<!-- 时间操作组件 -->
			<dependency>
				<groupId>joda-time</groupId>
				<artifactId>joda-time</artifactId>
				<version>${joda-time.version}</version>
			</dependency>
			<!-- Apache工具组件 -->
			<dependency>
				<groupId>org.apache.commons</groupId>
				<artifactId>commons-lang3</artifactId>
				<version>${commons-lang3.version}</version>
			</dependency>
			<dependency>
				<groupId>org.apache.commons</groupId>
				<artifactId>commons-io</artifactId>
				<version>${commons-io.version}</version>
			</dependency>
			<dependency>
				<groupId>commons-net</groupId>
				<artifactId>commons-net</artifactId>
				<version>${commons-net.version}</version>
			</dependency>
			<!-- Jackson Json处理工具包 -->
			<dependency>
				<groupId>com.fasterxml.jackson.core</groupId>
				<artifactId>jackson-databind</artifactId>
				<version>${jackson.version}</version>
			</dependency>
			<!-- httpclient -->
			<dependency>
				<groupId>org.apache.httpcomponents</groupId>
				<artifactId>httpclient</artifactId>
				<version>${httpclient.version}</version>
			</dependency>
			<!-- quartz任务调度框架 -->
			<dependency>
				<groupId>org.quartz-scheduler</groupId>
				<artifactId>quartz</artifactId>
				<version>${quartz.version}</version>
			</dependency>
			<!-- 单元测试 -->
			<dependency>
				<groupId>junit</groupId>
				<artifactId>junit</artifactId>
				<version>${junit.version}</version>
				<scope>test</scope>
			</dependency>
			<!-- 日志处理 -->
			<dependency>
				<groupId>org.slf4j</groupId>
				<artifactId>slf4j-log4j12</artifactId>
				<version>${slf4j.version}</version>
			</dependency>
			<!-- Mybatis -->
			<dependency>
				<groupId>org.mybatis</groupId>
				<artifactId>mybatis</artifactId>
				<version>${mybatis.version}</version>
			</dependency>
			<dependency>
				<groupId>org.mybatis</groupId>
				<artifactId>mybatis-spring</artifactId>
				<version>${mybatis.spring.version}</version>
			</dependency>
			<!-- 暂时没有用到 -->
			<dependency>
				<groupId>com.github.miemiedev</groupId>
				<artifactId>mybatis-paginator</artifactId>
				<version>${mybatis.paginator.version}</version>
			</dependency>
			<!-- 分页插件pagehelper -->
			<dependency>
				<groupId>com.github.pagehelper</groupId>
				<artifactId>pagehelper</artifactId>
				<version>${pagehelper.version}</version>
			</dependency>

			<!-- MySql -->
			<dependency>
				<groupId>mysql</groupId>
				<artifactId>mysql-connector-java</artifactId>
				<version>${mysql.version}</version>
			</dependency>
			<!-- 连接池 -->
			<dependency>
				<groupId>com.alibaba</groupId>
				<artifactId>druid</artifactId>
				<version>${druid.version}</version>
			</dependency>
			<!-- Spring -->
			<dependency>
				<groupId>org.springframework</groupId>
				<artifactId>spring-context</artifactId>
				<version>${spring.version}</version>
			</dependency>
			<dependency>
				<groupId>org.springframework</groupId>
				<artifactId>spring-beans</artifactId>
				<version>${spring.version}</version>
			</dependency>
			<dependency>
				<groupId>org.springframework</groupId>
				<artifactId>spring-webmvc</artifactId>
				<version>${spring.version}</version>
			</dependency>
			<dependency>
				<groupId>org.springframework</groupId>
				<artifactId>spring-jdbc</artifactId>
				<version>${spring.version}</version>
			</dependency>
			<dependency>
				<groupId>org.springframework</groupId>
				<artifactId>spring-aspects</artifactId>
				<version>${spring.version}</version>
			</dependency>
			<dependency>
				<groupId>org.springframework</groupId>
				<artifactId>spring-jms</artifactId>
				<version>${spring.version}</version>
			</dependency>
			<dependency>
				<groupId>org.springframework</groupId>
				<artifactId>spring-context-support</artifactId>
				<version>${spring.version}</version>
			</dependency>
			<!-- JSP相关 -->
			<dependency>
				<groupId>jstl</groupId>
				<artifactId>jstl</artifactId>
				<version>${jstl.version}</version>
			</dependency>
			<dependency>
				<groupId>javax.servlet</groupId>
				<artifactId>servlet-api</artifactId>
				<version>${servlet-api.version}</version>
				<scope>provided</scope>
			</dependency>
			<dependency>
				<groupId>javax.servlet</groupId>
				<artifactId>jsp-api</artifactId>
				<version>${jsp-api.version}</version>
				<scope>provided</scope>
			</dependency>
			<!-- 文件上传组件 -->
			<dependency>
				<groupId>commons-fileupload</groupId>
				<artifactId>commons-fileupload</artifactId>
				<version>${commons-fileupload.version}</version>
			</dependency>
			<!-- Redis客户端 -->
			<dependency>
				<groupId>redis.clients</groupId>
				<artifactId>jedis</artifactId>
				<version>${jedis.version}</version>
			</dependency>
			<!-- solr客户端 -->
			<dependency>
				<groupId>org.apache.solr</groupId>
				<artifactId>solr-solrj</artifactId>
				<version>${solrj.version}</version>
			</dependency>
			<!-- dubbo相关 -->
			<dependency>
				<groupId>com.alibaba</groupId>
				<artifactId>dubbo</artifactId>
				<version>${dubbo.version}</version>
			</dependency>
			<dependency>
				<groupId>org.apache.zookeeper</groupId>
				<artifactId>zookeeper</artifactId>
				<version>${zookeeper.version}</version>
			</dependency>
			<dependency>
				<groupId>com.github.sgroschupf</groupId>
				<artifactId>zkclient</artifactId>
				<version>${zkclient.version}</version>
			</dependency>
			<!-- activemq -->
			<dependency>
				<groupId>org.apache.activemq</groupId>
				<artifactId>activemq-all</artifactId>
				<version>${activemq.version}</version>
			</dependency>
			<dependency>
				<groupId>org.freemarker</groupId>
				<artifactId>freemarker</artifactId>
				<version>${freemarker.version}</version>
			</dependency>
		</dependencies>
	</dependencyManagement>

	<build>
		<finalName>${project.artifactId}</finalName>
		<plugins>
			<!-- 资源文件拷贝插件 -->
			<plugin>
				<groupId>org.apache.maven.plugins</groupId>
				<artifactId>maven-resources-plugin</artifactId>
				<version>2.7</version>
				<configuration>
					<encoding>UTF-8</encoding>
				</configuration>
			</plugin>
			<!-- java编译插件 -->
			<plugin>
				<groupId>org.apache.maven.plugins</groupId>
				<artifactId>maven-compiler-plugin</artifactId>
				<version>3.2</version>
				<configuration>
					<source>1.7</source>
					<target>1.7</target>
					<encoding>UTF-8</encoding>
				</configuration>
			</plugin>
		</plugins>
		<!-- 统一管理版本 -->
		<pluginManagement>
			<plugins>
				<!-- 配置Tomcat插件 -->
				<plugin>
					<groupId>org.apache.tomcat.maven</groupId>
					<artifactId>tomcat7-maven-plugin</artifactId>
					<version>2.2</version>
				</plugin>

				<!-- 配置打包时跳过测试 ，首次配置使用的时候会自动联网进行下载 -->
				<plugin>
					<groupId>org.apache.maven.plugins</groupId>
					<artifactId>maven-surefire-plugin</artifactId>
					<version>2.12.4</version>
				</plugin>
			</plugins>
		</pluginManagement>
	</build>
</project>
```
