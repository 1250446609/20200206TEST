测试本地项目上传到github gitlab


hm@LAPTOP-JEUTT4L2 MINGW64 /d/work/jialong
$ mkdir TEST

hm@LAPTOP-JEUTT4L2 MINGW64 /d/work/jialong
$ cd TEST/

hm@LAPTOP-JEUTT4L2 MINGW64 /d/work/jialong/TEST
$ git init
Initialized empty Git repository in D:/work/jialong/TEST/.git/

hm@LAPTOP-JEUTT4L2 MINGW64 /d/work/jialong/TEST (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        readme.txt

nothing added to commit but untracked files present (use "git add" to track)

hm@LAPTOP-JEUTT4L2 MINGW64 /d/work/jialong/TEST (master)
$ git add .

hm@LAPTOP-JEUTT4L2 MINGW64 /d/work/jialong/TEST (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   readme.txt


hm@LAPTOP-JEUTT4L2 MINGW64 /d/work/jialong/TEST (master)
$ git commit
Aborting commit due to empty commit message.

hm@LAPTOP-JEUTT4L2 MINGW64 /d/work/jialong/TEST (master)
$ git commit -m "第一次提交"
[master (root-commit) 606500b] 第一次提交
 1 file changed, 1 insertion(+)
 create mode 100644 readme.txt

hm@LAPTOP-JEUTT4L2 MINGW64 /d/work/jialong/TEST (master)
$ ssh-keygen
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/hm/.ssh/id_rsa):

hm@LAPTOP-JEUTT4L2 MINGW64 /d/work/jialong/TEST (master)
$ ssh-keygen -t rsa -C "1250446609@qq.com"
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/hm/.ssh/id_rsa):
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /c/Users/hm/.ssh/id_rsa.
Your public key has been saved in /c/Users/hm/.ssh/id_rsa.pub.
The key fingerprint is:
SHA256:cvAyDP3ul7R8d84LSnTyUBfn1hXMQEpz+Q4dQnxfCS4 1250446609@qq.com
The key's randomart image is:
+---[RSA 3072]----+
|           o+**o=|
|     .    . =+ B*|
|    . o    E o=.B|
|     o +    o..+.|
|      = S  + .o  |
|       *  o =  . |
|        .o + o   |
|       .  * o o..|
|        .. o . ++|
+----[SHA256]-----+

hm@LAPTOP-JEUTT4L2 MINGW64 /d/work/jialong/TEST (master)
$ git remote add origin https://github.com/1250446609/20200206TEST.git

hm@LAPTOP-JEUTT4L2 MINGW64 /d/work/jialong/TEST (master)
$ git push -u origin master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 257 bytes | 257.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/1250446609/20200206TEST.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.
