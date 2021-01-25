## Powershell
-> mkdir - creates a new directory

-> cd - changes the directory

-> cd .. - changes to root directory

-> ni - creates new item

-> rm - removes an item

-> ls - list the items

-> ALT SPACE C -To close the window


## Some of the Gitbash commands
-> git branch branchName - creates a new branch

-> git branch - lists all the branches

-> git clone repoUrl - clones the cloud repo to local machine

-> git pull origin branchName - pulls the fresh code from repo

-> git add remote origin repoUrl - adds remote folders to cloud repo

-> git add . - adds the files

-> git commit -m "initial commit" - commits to the repository

-> git push origin branchName - pushes the changes to that specified branch

-> head -5 filename.txt - displays the top 5 lines of file

Process the text data using Bash commands :

1)Transform each space ' ' into a return character '\12' (aka ASCII line feed)
	tr ' ' '\12' < data.txt

2)Pipe the output to sort (send the results of one command as input into another command)
	tr ' ' '\12' < data.txt | sort
	
3)Pipe the sorted output to uniq -c to count
	tr ' ' '\12' < data.txt | sort | uniq -c
	
4)Pipe the reduced output to sort with -nr flag
	tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr
	
5)Redirect the output to result.txt
	tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr > result.txt
