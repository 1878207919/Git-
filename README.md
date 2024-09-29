# Git-
学习Git使用的笔记
## 新建仓库
1、在Git Demo中新建一个文本文档test.txt，用Git Bash打开
2、输入git init,初始化成一个空的仓库
## 导入文件
3、向缓冲区添加新文件输入：git add test.txt，输入git status查看缓存区状态,发现缓冲区出现新文件，若要删除缓存，输入git rm --cached
4、输入git commit -m ”first commit“，将文件 text.txt 提交到了 Git 仓库。其中，-m代表提交信息，“first commit”是本次提交的信息，需要写在双引号内，提交信息你也可以写成my commit，text commit等任意句子
5、输入git log命令，打印Git仓库提交日志，会显示作者、时间和写的提交信息
## 分支建立转换查看
6、输入git branch，查看在哪个分支上
7、新建分支用 git branch a，用 git branch 查看
8、输入 git checkout a 命令，切换到分支 a 上，再次查看分支
## 合并
9、先切换到master中，再git merge a
10、a合并到master中，就删除分支a，git branch -d a
## 标签
11、git tag v1 代表新建 v1 ta
12、git checkout v1检查
## git hub
1、输入 ssh-keygen -t rsa （指定 rsa 算法生成密钥），接着连续三个回车键（不需要输入密码），然后就会生成两个文件 id_rsa （密钥）和 id_rsa.pub （公钥）
2、把 id_rsa.pub 的内容添加到 GitHub 上，这样你本地的 id_rsa 密钥跟 GitHub 上的 id_rsa.pub 公钥进行配对，授权成功才可以提交代码
3、在git bash 中输入ssh-T git@github.com
