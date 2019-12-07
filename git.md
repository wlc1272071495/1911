

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
<!-- 工作区 => 提交到暂存区   显示绿色 -->
<!-- 工作区 => 没有提交到暂存区   显示红色 -->

<!-- 比较工作区 和 暂存区 git diff 文件名 -->
<!-- 从暂存区  撤回到  工作区  git checkout  文件名 -->

<!-- 统一将暂存区中的所有修改提交到 版本库 -->
git commit -m "初始化提交"

<!-- 提交日志  -->
git log

<!-- 重复提交 还是按照上述步骤 -->


<!-- 创建分支   -->
git  branch 分支名

<!-- 切换分支   -->
git checkout 分支名

<!-- 简写  创建并切换  -->
git branch -b dev 
