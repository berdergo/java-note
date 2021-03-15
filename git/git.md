



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


# 回退到 commit_id 指定的提交版本
git reset --hard 'commit_id'


# 操作历史命令 可以查找回退之前的ID
git reflog


# 删除版本库中的文件
git rm test.txt
git commit
```



### 分支管理

```bash
# 查看本地分支信息 
git branch 
# 查看相对详细的本地分支信息 
git branch -v 
# 查看包括远程仓库在内的分支信息 
git branch -av


# 新建一个名称为 dev 的分支 
git branch dev

# 新建完 dev 分支以后，通过该命令切换到 dev 分支 
git checkout dev

# 新建 dev 分支，并切换到该分支上 
git checkout -b dev



# 切换回 master 分支 
git checkout master 
# 将 dev 分钟中的修改合并回 master 分支 
git merge dev

# 删除 dev 分支 
git branch -d dev
```

