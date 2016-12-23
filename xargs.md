xargs 将标准输入转换为命令行参数

与find结合使用
``` bash
$ find . -type f -name "*.txt" -print0 | xargs -0 rm -f
```

替换字符串
cat files.txt | xargs -I { } cat { }