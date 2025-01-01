hint: since we trying to focus on git commands i dont' mention cd commands and ls in cli 
1- First before we start version control we fork repository 
2- try to clone repository by the command of
     "git clone git@github.com:HoesienZR/PGU_ResourceSharing.git" 
3- then we create a new branch and start our changes by the command 
    "git Branch  HoesienZR"
    "git checkout HoesienZR"
4- then we add our changes to our branch whatever is our changes is 
5- use "git status" to see what changes is not staged 
6- after see what changes is not we use add command to add our file in staging like the following 
    "git add Notes.md"
7-but if we have any problem to add our files since maybe we have like Test 1.md 
and git can't add our file like this we put our file in Double qoute like this 
    git add "Test 1.md"
8-after we add our file we commit it using command 
    git commit -m "added notes in OS in HoesienZR directory" 
9-and after our changes all are committed it's time to push changes to our directory 
    "git push origin"
10- after that we opne a pull request and merge our changes to the main branch :D 
