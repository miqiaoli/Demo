# Linux

## 一. Linux目录说明：

![Linux目录](./assets/linux.png)

## 二. Linux常用命令：
1. 目录
   1. 查看目录：`ls`
   2. 进入目录：`cd`
   3. 快捷操作：
      1. 向上：`cd..`
      2. 后退：`cd-`
      3. 回到home：`cd~`
      4. 回到根目录：`cd/`
   4. 查看目录结构： `tree`
   5. 新建目录：`mkdir`
      1. 多级目录：`mkdir -p one/two/three`
   6. 复制：`cp -r 原目录 目标目录`
   7. 删除：`rm -r`
2. 文件：
   1. 新建：`touch`
   2. 复制：`cp 文件名 目的路径`
   3. 删除：`rm 文件名`
   4. 移动/重命名：`mv 文件名`
   5. 查看：`cat`
   6. 编辑：
      1. `vim`
      2. `sublime/gedit`
      3. 其他
3. 后续
   。。。


## 三. Git操作：
1. 基本操作：
   1. `git init`
   2. `git config --global user.name  用户名`
   3. `git config --global user.email 邮箱`
2. 提交代码流程：
   1. `git add .`
   2. `git commit -m 'first commit'`
3. 链接远端仓库：
   1. `git remote add origin url`
   2. `git pull`
   3. `git push`