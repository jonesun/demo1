# demo1

使用了spring boot 2.4.2版本的话，需要手动在配置文件application.yml中加入:

```yaml
logging:
  charset:
    console: gbk
```
否则打包成jar后，在windows下，输出日志中存在中文的话，会出现乱码
