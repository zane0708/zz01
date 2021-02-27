# Git命令

## 1.仓库初始化

``` 
git init
```

## 2.添加到暂存区

```
git add 文件名字
```

## 3.提交到仓库

```
git commit -m "文件描述"
```

## 4.查看状态

```
git status
git status -s //精简
```

## 5.撤销对文件的修改

```
git checkout -- 文件名
```

## 6.取消暂存的文件

```
git rest HEAD 文件名
git rest HEAD . //取消全部
```

## 7.跳过暂存区

```
git commit -a -m "文件描述"
```





## 8.移除文件

从 Git 仓库中移除文件的方式有两种：

① 从 Git 仓库和工作区中**同时移除**对应的文件

② 只从 Git 仓库中移除指定的文件，但保留工作区中对应的文件

```shell
# 从 Git仓库和工作区中同时移除 index.js 文件
git rm -f index.js
# 只从 Git 仓库中移除 index.css，但保留工作区中的 index.css 文件
git rm --cached index.css
```