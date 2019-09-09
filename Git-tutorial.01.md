## This is a tutorial to clone and keep updates of the forked repo (Win10)
### 1. Open your [Git BASH](https://gitforwindows.org/) and Clone your fork 
- [username/ATM651_IntroAtmDynamics](https://github.com/kathy9980/ATM651_IntroAtmDynamics) - This is my example

  `git clone https://github.com/[username]/ATM651_IntroAtmDynamics`
- change to the forked repository on your hard drive
  
  `cd ATM651_IntroAtmDynamics`
  
### 2. Add remote from original repository in your forked repository
  #### 1. [`git remote`: Manage set of tracked repositories](https://git-scm.com/docs/git-remote)
```
  git remote add origin https://github.com/[username]/ATM651_IntroAtmDynamics   
  git remote add upstream https://github.com/ATMOcanes/ATM651_IntroAtmDynamics
```
Now, run `git remote -v`, you will have an output like this:
```
origin  https://github.com/[username]/ATM651_IntroAtmDynamics.git (fetch)
origin  https://github.com/[username]/ATM651_IntroAtmDynamics.git (push)
upstream        https://github.com/ATMOcanes/ATM651_IntroAtmDynamics.git (fetch)
upstream        https://github.com/ATMOcanes/ATM651_IntroAtmDynamics.git (push)
```
  #### 2. [`git fetch`: Download objects and refs from another repository](https://git-scm.com/docs/git-fetch)
```
  git fetch upstream
``` 
### 3. Updating your fork from original repo to keep up with their changes:
```
  git pull upstream master
```
Let's check if we have the latest update `TAexam.md` from the upstream.
```
ls
ATM651_conda_environment.yml  README.md
calendar.md                   Syllabus_ATM651_Graduate_Intro_Dyn_2019.pdf
INSTALL_SOFTWARE.md           TAexam.md
LICENSE                       Unit1-Terminology_and_Tools/
```
Yeah! Up to date!

This tutoridal is based on Wei-ming's lecture and [CristinaSolana's notebook](https://gist.github.com/CristinaSolana/1885435#file-gistfile1-md).
09/09/2019