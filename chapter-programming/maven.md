# Maven

## 中心仓库配置

配置文件位置：

1. $MAVEN_HOME/conf/settings.xml
1. $HOME/.m2/settings.xml

```xml
<mirror>
  <id>alimaven</id>
  <mirrorOf>central</mirrorOf>
  <name>aliyun maven</name>
  <url>http://maven.aliyun.com/nexus/content/repositories/central/</url>
</mirror>
```

## 测试

指定测试某一类或某一方法

```Shell
mvn test -Dtest=PagedFileTest
```

```Shell
mvn test -Dtest=PagedFileTest#disposePage
```

## 实用工具

### 分析不需要的依赖

使用 maven-dependency-plugin，定义 `dependency:analyze` goal，可以分析 pom.xml 中有哪些依赖实际上没有用到。

## 其他注意事项

Mac OS 遇到 Spring Boot 启动慢的事情，可能是因为 host 解析很慢。解决方法：

第一步，运行 `hostname` 命令，记下来本机名称（如 MacBook.local）。

第二步，修改 `/etc/hosts` 文件

```
127.0.0.1    localhost    MacBook.local
::1          localhost    MacBook.local
```