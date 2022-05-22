## 背景

由于windows上的文件结束符和linux上有所不同，那么在windows上编写的文件或者是脚本在linus会遇到类似的问题

```
/bin/sh^M: bad interpreter: No such file or directory
```

出现这个问题是因为结束符不同，要解决上诉问题，只需要转换下文件类型就行

## 针对单个文件或者少量文件

```shell
# 通过vim打开该文件
vim file
# 设置unix的格式
：set fileformat=unix
# 设置windows的格式
：set fileformat=dos
# 查看文件格式类型
: set ff
```

## 批量修改多文件

上面的适合文件较少，如果文件较多，可以利用如下的方法

```shell
# 文件名与文件类型更改成自己要修改的就行
sudo find ~/.cache -name "*.vim" | xargs dos2unix		
```

