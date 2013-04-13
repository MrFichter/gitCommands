
TO ADD NEW REPO TO GIT FROM COMMAND LINE: 

git remote add origin ssh://url.to/githubrepository  

# example, I think: 

# git remote add origin ssh://https://github.com/MrFichter/pygameTest

git push

OR: follow the steps below. They are similar but use https instead of the ssh 
(THIS IS WHAT GITHUB RECOMMENDS)

https://help.github.com/articles/create-a-repo

NOTE: You need to go to github.com to create a repo before you do this.

After that, you can just do git push





SETTING UP AN SSH KEY SO THAT YOU DON’T HAVE TO ENTER A PASSWORD


cd #to get to home directory

mkdir .ssh #if it doesn’t exist already

cd .ssh

ssh-keygen  #generates a pair of public and private keys

[press Enter to opt out of other things a few times]

cat id_rsa.pub #highlight with mouse and use control + shift + c to copy. then go to github settings in your browser and add


vim .git/config   #for a given repo, copy from browser the ssh stuff and \
#paste it over the https stuff



GIT CLONE WHEN YOU WANT TO BE ABLE TO PUSH TO IT

git clone https://mrfichter@github.com/MrFichter/FutureProjectIdeas.git




TO MODIFY AN EXISTING REPO AFTER CLONING: 

git push https://github.com/MrFichter/FutureProjectIdeas.git (you can see this by clicking the http tab on the github website. it’s case sensitive.)





GIT LOG

git log --grep “search term” searches your git log. It’s case sensitive, though.

example: git log --grep “Learning”
git log -i --grep “learning” 

the -i makes it case-insensitive
you can also type git log to see everything. then press q to get back into command mode

Git log: if you’re writing a longer paragraph, you can press enter whenever you want.

