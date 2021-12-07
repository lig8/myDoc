###  命令读写文本

1、创建一个空件

``` bash
touch abc.md
```
2、将文本写入一个文件，文件不存在会创建这个文件

```bash

echo 'hello world' > abc.md
```

3、将文本追加到一个文件

```bash

echo 'hello python' >>abc.md
```

4、显示一个文件的内容
```bash

cat abc.md
# more for dispaly in page
cat abc.md | more
```







