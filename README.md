# demo1

使用了spring boot 2.4.2版本打包成jar后，使用java -jar xxx.jar, 在windows控制台运行, 如果输出日志中存在中文的话，会出现乱码

https://github.com/spring-projects/spring-boot/issues/24894

解决方法是:

手动在配置文件application.yml中加入:

```yaml
logging:
  charset:
    console: gbk
```
