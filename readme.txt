
TO ADD NEW REPO TO GIT FROM COMMAND LINE: 



create new repo on github.com

create directory

git init

create readme

git add readme

git commit

git remote add origin git@github.com:MrFichter/FutureProjectIdeas.git

[add ssh key if you haven’t added for this computer key]

vim .git/config   #for a given repo, copy from browser the ssh stuff and \
#paste it over the https stuff
git push -u origin master 

# The -u option automatically sets that upstream for you, linking your repo to a central one. That way, in the future, Git "knows" where you want to push to and where you want to pull from, so you can use git pull or git push without arguments. (from http://stackoverflow.com/questions/5561295/what-does-git-push-u-mean)



all of the above is described here
https://help.github.com/articles/create-a-repo




GIT CLONE WITH HTTPS. BEST OPTION IF YOUR PC DOES NOT HAVE
AN SSH KEY.

git clone https://mrfichter@github.com/MrFichter/FutureProjectIdeas.git






SETTING UP AN SSH KEY SO THAT YOU DON’T HAVE TO ENTER A PASSWORD


----(IF YOU DON’T ALREADY HAVE AN SSH KEY)


cd #to get to home directory

mkdir .ssh #if it doesn’t exist already


cd .ssh


ssh-keygen  #generates a pair of public and private keys

[press Enter to opt out of other things a few times]


cat id_rsa.pub #highlight with mouse and use control + shift + c to copy. then go to the main github settings in your browser and add, naming your new computer



GIT CLONE. BEST OPTION WHEN YOU HAVE AN SSH KEY.

git clone git://github.com/MrFichter/FutureProjectIdeas (case sensitive)






TO MODIFY AN EXISTING REPO AFTER CLONING: 

git push https://github.com/MrFichter/FutureProjectIdeas.git (you can see this by clicking the http tab on the github website. it’s case sensitive.)





GIT LOG

git log --grep “search term” searches your git log. It’s case sensitive, though.

example: git log --grep “Learning”
git log -i --grep “learning” 

the -i makes it case-insensitive
you can also type git log to see everything. then press q to get back into command mode

Git log: if you’re writing a longer paragraph, you can press enter whenever you want.

