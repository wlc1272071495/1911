

1. 安装git  

2. 注册  gitHub  和   码云账号

1. 设置用户名和邮箱
    git config --global user.name "www";

    git config --global user.email "1272071495@qq.com";


2. 初始化本地仓库
git init   

3. 将本地文件提交到 暂存区
git add .

git status   查看提交的状态

<!-- 统一将暂存区中的所有修改提交到 版本库 -->
git commit -m "初始化提交"

<!-- 提交日志  -->
git log 