



## 基本配置

```bash
# 配置用户信息
git config --global user.name berdego
git config --global user.email xinfeng365@126.com
# 显示基本配置信息
git config --list
```





## 构建本地仓库

```bash
# 初始化本地仓库
git init
# 查看当前文件状态
git status [-s]

# 添加单个文件到暂存区 
git add Readme.txt
# 将当前目录下所有修改添加到暂存区，除按照规则忽略的之外 
git add .

# 如果暂存区所有文件，则将其中的文件提交到仓库 
git commit

# 带评论提交，用于说明提交内容、变更、作用等 
git commit -m 'your comments'


# 显示所有提交的历史记录
git log
# 单行显示提交历史记录的内容
git log --pretty=oneline 
```



