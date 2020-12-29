# apiggs-maven-plugin
[ ![Download](https://api.bintray.com/packages/apiggs/maven/apiggs-maven-plugin/images/download.svg) ](https://bintray.com/apiggs/maven/apiggs-maven-plugin/_latestVersion)

easy use apigcc with maven

### install
```xml
<plugin>
    <groupId>com.github.apiggs</groupId>
    <artifactId>apiggs-maven-plugin</artifactId>
    <version><!-- 替换为上方版本号 --></version>
    <executions>
        <execution>
            <phase>compile</phase>
            <goals>
                <goal>apiggs</goal>
            </goals>
        </execution>
    </executions>
    <configuration>
        <!-- options in there -->
    </configuration>
</plugin>
```

when you compile source code, apiggs will build rest doc.

### options

1. id 项目id，生成id.html文件
1. title 文档标题
1. description 文档描述
1. production 输出文件夹，默认为 apiggs
1. out 输出目录，默认为 target
1. source 源码目录
1. dependency 源码依赖的代码目录，以逗号隔开
1. jar 源码依赖的jar包目录，以逗号隔开
1. ignore 忽略某些类型
1. version 文档版本号
1. urlPrefix 生成url时添加的前缀