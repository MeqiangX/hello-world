# hello-world
This is a simple demo of github repository

# 学习github
1. 创建repository and 创建项目
  1. 从github web 上创建
  
    > 直接将本地项目 拖入 (但是要小于100个文件)
    
  2. 从git bash 上 创建
  
    1. 打开git bush  配置上user.name 和 user.email 为github 创建时候的 账号和邮箱
    
      > git config --global user.name "MeqiangX"
      > git config --global user.email "xiaoqiang9611@gmail.com"
      
    2. 设置SSH key
    3. 生成ssh key 
       > 检查是否已经生成了秘钥 cd ~/.ssh 如果返回了三个文件 则生成了 但是也要注意是否是 上次配置时候的账户和邮箱生成的，如果是则需要重新配置之后再次生成
       > 如果没有或者需要重新生成则通过： ssh-keygen -t rsa -C "xiaoqiang9611@gmail.com" 过程按默认的就好 然后生成之后打开 id_rsa.pub 的秘钥 copy到github 的add sshkey 
       
    4. 完成上述步骤之后就可以开始 创建本地仓库了
    
      1. 进入要项目目录
      2. 执行 git init 初始化本地仓库 会发现多了一个.git 版本控制文件夹
      3. 执行 git add .将所有文件添加到仓库 (git init 之后 创建了一个空的.git 而.git是不能管理空文件夹的，需要add .将当前文件夹所有的文件都交由.git来管理)
      4. 执行 git commit -m '注释提交文件' 提交
      5. 关联github 仓库
      
        > 到github 的项目repository 复制仓库地址 (注意 这里是要在创建仓库的时候不勾选add readme.md 从已经有的本地仓库中导入) 执行命令 : git remote add origin https://github.com/MeqiangX/mediamanagesys-parent.git 然后上传本地代码到远程仓库 git push -u origin master 
      
     6. finshed 可以在远程仓库上看到我们的项目了
     
     7. 之后就可以创建分支 拉取 然后操作了
      
    
