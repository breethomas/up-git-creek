### WIP Git Creek Cheat Sheets

- basic workflows
- common issues and solutions
- maybe one day this will become a gorgeous decision tree graphic, complete with adorable illustrations

#### And so our story begins...

# Falling In Love with Git in Six Acts 
**(inspired by [Nike's 1993 Vanity Fair Ad](http://www.rogerhorberry.com/falling-in-love-in-six-acts-courtesy-of-nike/))**

##1. LUST :heart_eyes:
Here it is, the big “Wow!” the big “Gee!” the big “YesYesYes!” you’ve been waiting for...**YOU HAVE A NEW PROJECT ASSIGNMENT**. This is where you decide to build something better, greater, cuter, wiser, more wonderful than anything anyone has ever known. Lust isn’t a sin, it’s a necessity, for with lust as our guide we think: I have no need of food, I have no need of sleep, I have no needs other than occasionally chewing a breath mint. I am going to code my face off. And so it begins...

*There are two paths to the start of this journey. You must be comfortable in both.*

### Path-A) I create my project on the big Github :octocat: in the sky first:

- I visit my profile on GH and I create a new repo, following these [steps](https://help.github.com/articles/creating-a-new-repository/).
- Yay! I will now clone this very shiny new, empty repository onto my machine. And the lovely GH provides the [steps](https://help.github.com/articles/cloning-a-repository/) to do so.
- I do not have to ```git init``` in ```<my-awesome-project-name>```. Because I cloned from the big GH in the sky, I am all initialized with an empty .git repository. I am special. :tulip:
- And just to be sure all is well, I will double check that the project on my machine is in fact connected to the big :octocat: in the sky.
```
cd <my-awesome-project-name>
git remote -v
```
Eeeeeeeee!!!! :clap: Life is so good, because this:
```
# origin	git@github.com:you/my-awesome-project-name.git (fetch)
# origin	git@github.com:you/my-awesome-project-name.git (push)
```
I have the correct remotes in place for my local machine to both push and fetch from the big :octocat: in the sky.:thumbsup:

### Path-B) I create my project locally first:
```
mkdir <my-awesome-project-name>
cd <my-awesome-project-name>
git init
```
Boom. :boom: ```#Initialized empty Git repository in /Users/you/my-awesome-project-name/.git```

I want to share the love with everyone!!! How do I do this? OH RIGHT! I push my project up :arrow_up: to the big Github :octocat: in the sky. I will go there now and follow these [steps](https://help.github.com/articles/creating-a-new-repository/) to create a new repository.

:speech_balloon: BUT WAIT! Can they talk to one another? Is the project on my machine connected to my github repo? :confused: I get that for free when I clone from Github like in Path-A, but because I chose Path-B, I must create the connection between the two entities. I will do it. :muscle:
```
cd <my-awesome-project-name>
git remote -v  
(#see that it it empty, nothing happens)
git remote add origin git@github.com:you/my-awesome-project-name.git 
(#copy paste the GH url of your project and assign it to the label of 'origin')
git remote -v 
(#check that you have the remotes)
```
You are ready to Rock and Roll. :microphone: :guitar:
##2. EUPHORIA :lollipop:
You feel funny inside. You feel funny outside. You feel you could do anything and no one would dare laugh at you. This git and github, you will treasure. You will not put it in the basement next to your rowing machine, treadmill, and thermal body sweat wrap. And you will not take the git for granted, because that is the biggest sin of all. You will commit. And commit often. You will make your first commit like no other. Because you are solo. This is your repo, your project, your one-person-in-charge-of-every-last-commit-domain. 

### You are making changes and coding things:
```
git status
(# prints the status of your current situation.)
(# expect git to tell you what you branch you are on and which files are "untracked", meaning changes were made)
git add .
(# this command will add ALL the changes you just made to "staging", meaning they are ready to be committed)
git add <path/filename>
(# this command will add changes based upon the file you specify)
git status
(# run this command after EVERY git command to reinforce that you know what you are doing and where you are at any git-moment)
```
### You are ready to commit:
```
git status
(# you have changed files that are "staged" and ready for commit)
git commit -m "My awesome commit message"
(# you are happy with your staged changes and commit them with no apology)
git status
(# at this juncture, you might see "nothing to commit, working tree clean")
```
### You want to share your masterpiece with the world:



##3. FEAR :see_no_evil:

##4. DISGUST :poop:

##5. TRUTH :raised_hands:

##6. FINALE :sparkling_heart:
