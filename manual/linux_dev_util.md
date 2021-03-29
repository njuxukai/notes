# shell命令

批量转换文件格式

```shell
find . -name "hello.cc" -exec dos2unix {} \;
find . -name "*.h" -exec dos2unix {} \;
find . -name "*.sh" -exec dos2unix {} \;
```

