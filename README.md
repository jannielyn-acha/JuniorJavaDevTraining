{\rtf1\ansi\ansicpg1252\cocoartf2580
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fmodern\fcharset0 Courier;}
{\colortbl;\red255\green255\blue255;\red0\green0\blue0;}
{\*\expandedcolortbl;;\cssrgb\c0\c0\c0;}
\margl1440\margr1440\vieww19280\viewh11440\viewkind0
\deftab720
\pard\pardeftab720\partightenfactor0

\f0\fs24 \cf2 \expnd0\expndtw0\kerning0
\outl0\strokewidth0 \strokec2 # Hands-on Activity\
This hands-on activity is to gauge your knowledge in Versioning.\
\
1. Clone this repository.\
2. Edit `Hello.txt` and append the content with your name in it.\
3. Create a new text file and name it according to your name. Leave it blank.\
\
	#### Question#1\
	1. If we want to check the modified/untracked files, what git command should you execute?  \
	2. What is/are the name(s) of the **untracked** file(s)?  \
___\
\
4.  Stage and commit only the `Hello.txt` file. Any commit message would do.\
\
	#### Question#2\
	1. What command(s) did you use to stage and commit `Hello.txt` file?\
	2. Where is the committed file located after you execute the command - (A) Local Repository or (B) Remote Repository or (C) None of the above? (Letter only!)\
	3. How about the staged file, where is it located - (A) Local Repository or (B) Remote Repository or (C\\) None of the above? (Letter only!)\
---\
5. Edit again `Hello.txt` by adding your year and course next to your name and commit the said file. Again, any commit message would do.\
6. Stage and commit **all** **unstaged** files (meaning, all modified / untracked files).\
\
	#### Question#3\
	1. What is/are the commands you used in stage-committing all the files **at once**? (Regardless of there status i.e. untracked, modified, etc.)\
	2. Can you amend/change the commit message after committing it? If yes, how? If no, why? (If yes, name the command(s))\
---\
\
7. Check the logs.\
\
	#### Question#4\
	1. What is the first commit's hash code?\
	2. What is the command to display up to 2 recent logs?\
	3. (**Bonus!**) Write the default keyboard inputs when browsing/exiting in the log in the command line/git bash.  \
			a. Move page up.  \
			b. Move page down.  \
			c. Move to next line.  \
			d. Move to previous line.  \
			e. Exit log.  \
---\
8. Edit `Hello.txt` and add today's date(any date format) next to your course.\
9. Edit the file you created before (file containing your name as its filename), add your school's name in it.\
10. Commit all modified files.\
11. Un-commit your last committed files (Not amend the commit message!). Changes should retain!\
	\
	#### Question#5\
	1. Instead of retaining the changes from the previous step (Step#11), we want to  discard the changes in the committed file(s) (hard), what command is that?\
	2. (**Bonus!**) Can you un-commit up to 2 commits? If so, what command(s) should you use to achieve that?\
---\
\
12. Unstage `Hello.txt` file.\
13. Remove all local changes in `Hello.txt` file\
\
	#### Question#6\
	1. Where is the `Hello.txt` file located before removing all local changes in it? - (A) Working directory, (B) Staging area (C\\) Local Repository (D) Remote Repository (E) None. (Letter only!)\
	2. Suppose you have 10 modified local files, how do you remove the local changes all **at once**?\
	3. (**Bonus!**) Suppose you deleted a file and you want to undo it, what command should you use? (**Clue:** Checkout your HEAD)\
---\
14.  Commit all staged file(s).\
15. Create a local branch and name it `<your name>-feature` branch.\
16.  Move to that branch and push it.\
		\
		#### Question#7\
		1. Two ways to create a new branch?\
		2. If one of the mentors wants to get a copy of your newly pushed branch to his local, what command should he use in order to download contents from the remote repository?\
		3. What is the command to list down all local branches?\
		4. (**Bonus!**) How about list down all remote branches?\
		5. Suppose you go back to master/main branch and delete your local `<your name>-feature` branch, can you still move back to your local branch?  \
			a. If yes, will it automatically create a local branch by simply checking it out?  \
			b. If no, do you still need to create a new branch bearing the name `<your name>-feature` branch?  \
---\
17. Go back to master/main branch.\
18. Delete your newly created local branch `<your name>-feature-branch`.\
19. Edit `Hello.txt` by adding your favorite number before your name.\
20. Move your changes to another new branch. Name it `<your name>-task` branch.\
\
	#### Question#8\
	1. How did you move your changes to another new branch without stashing them?\
	2. Can you move to an **existing** branch while having local changes in your working directory? Yes or No.\
---\
\
21. Commit `Hello.txt` and push it.\
22. Edit again `Hello.txt` file by clearing all the contents in it.\
23. Store your changes in a stash.\
\
	#### Question#9\
	1. What is the command to execute if you want to store your local changes in a stash?\
	2. (**Bonus! Data Struct Refresher**) Stash follows the principle of  LIFO(FILO) or LILO(FIFO)?\
---\
24. Fetch the remote branches of your fellow interns and checkout to their branch:\
\
| You | Branch Assignment |\
|:---:|:---:|\
| Arnan | Cloyd's branch |\
| Cloyd | Rayl's branch |\
| Rayl | Arnan's branch |\
\
e.g. Arnan -> will checkout to `cloyd-task` branch. \
**Note**: Wait for others if you cannot fetch their remote branch.\
\
25. Pop your stash code. Conflict will occur.\
\
	#### Question#10\
	1. What happens to your stashed code after executing pop? (A) Retains the stashed code (B) Deletes the stashed code. (Letter only!)\
	2. What is the difference between `pop` and `apply`?\
	3. Since stash is a (depends on your answer in Question#9.2), can you execute `pop` to a specific index? If so, how?\
	4. Same question as above but using `apply`. If so, how?\
---\
26. Abort resolving the conflict using `git reset --merge`.\
27. Edit `Hello.txt` and remove the course and year in it.\
28. Commit and push  it to its origin branch (remote branch).\
29. Go back to main/master branch.\
30. Merge your own branch to  main/master branch. Resolve conflict(s) if deemed necessary.\
}