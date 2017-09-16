
1.	https://github.com/cuichanjie/AcademicStudy  用你的浏览器打开，并且github已登录的情况下，可以看到你的private项目。
2.	页面有个clone or download 点击后有个链接，https://github.com/cuichanjie/AcademicStudy.git ，在你的工作电脑上，git clone https://github.com/cuichanjie/AcademicStudy.git ,可以把代码下载下来，能看到AcademicStudy文件夹
3.	在AcademicStudy/，用git status可以看到提示：修改的文件，以及没有commit的文件。提交修改需要分两个步骤，先用git add your_modified_file_name，然后git commit –m “your comment for the modification”。如果修改的文件有多个，可以用git add –A，然后git commit –m “your comment for the modification”。
4.	将修改同步到github上: git push origin master，按照提示输入github用户名和密码。
5.	如果不想让git管理某个文件，可以编辑.gitignore文件，写上文件名，有必要的话加上文件路径。在.gitignore写入*.dat表示所有dat后缀的文件都被忽略。编译产生的二进制文件不需要托管到github上，所以一般会让git忽略掉这些文件。
6.	可以在上述第一步的链接里面，点击n commits，也就是进入https://github.com/cuichanjie/AcademicStudy/commits/master ，能看到commit的记录，点击某一次的commit，能看到做了哪些修改，某次commit最右边有个<>符号，点击进去你能看到以该次commit为历史截点的整个项目。所以你可以重新回到以前某个commit截点下的项目，不用担心改错代码找不到以前的版本。
7.	如果想基于现有代码，改动代码用于新的实验，同时想保留这两个版本的代码，可以新开一个分支(branch)。在https://github.com/cuichanjie/AcademicStudy ，页面上有个Branch: master，点击进入，输入分支名称，按照提示点击Create branch: 分支名。基于这个分支在本地来做修改，可以git clone https://github.com/cuichanjie/AcademicStudy.git -b 分支名。修改后，上传github，和上面基本相同，在本地先add再commit，然后用git push origin 分支名。上面用master是因为分支名是master。
8.	如果commit了一次修改，并且同步到了github上了，想撤销这次commit，可以参考https://stackoverflow.com/questions/448919/how-can-i-remove-a-commit-on-github
9.	如果在add一个修改文件之后，commit之前，想撤销add，可以参考https://stackoverflow.com/questions/348170/how-to-undo-git-add-before-commit
不过，你在本地的改动仍然还在，按照链接中的方法undo add后，用git status查看会提示这个文件修改了，而不是提示让你commit。

