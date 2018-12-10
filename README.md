# Project Title

One Paragraph of project description goes here

## Cheatsheet

```
$ git remote show origin
* remote origin
  Fetch URL: https://github.com/waikitman/sandbox-git.git
  Push  URL: https://github.com/waikitman/sandbox-git.git
  HEAD branch: master
  Remote branches:
    feature/sbf-1 tracked
    master        tracked
  Local branch configured for 'git pull':
    master merges with remote master
  Local refs configured for 'git push':
    feature/sbf-1 pushes to feature/sbf-1 (up to date)
    master        pushes to master        (up to date)
```

##### Viewing log

In scenario below.
* Add + commit file to testing branch. Switched to master.
* Add + commit file to master branch. Switched to develop.
* Add/modify + commit file to develop and ran git log command to see current state.

```
$ git log --oneline --decorate --graph --all
* df593b5 (HEAD -> develop) Add develop text file
| * d8459b3 (master) Add master-branch file
|/  
| * 384a451 (testing) Adding file from testing branch
|/  
* a89991e (origin/master, origin/develop, origin/HEAD) Changing comment in file
* 01d2b89 (tag: v0.0) Added a new wai file
| * a05147d (origin/feature/sbf-1) Added file for sbf-1 branch
|/  
* 47bb275 Add command to cheatsheet
* fcb3410 Added drupal 8 example.
*   8cab6dd Merge branch 'master' of https://github.com/waikitman/sandbox-git
|\  
| * 1ea2a2b Change README. Add a bunch of test markup.
* | 8a88590 (tag: v0.0-alpha) Change README. Add a bunch of test markup. Changed message using git --amend
|/  
* 8903a75 Initial commit
```

##### Check which branches have been merged or not.
```
$ git branch --merged
* develop
  testing
$ git branch --no-merged
  master
```

##### Deleting an un-merged branch.
```
$ git branch -d abcde
error: The branch 'abcde' is not fully merged.
If you are sure you want to delete it, run 'git branch -D abcde'.
```


### Remote branches


##### Create branch that tracks remote branch of the same name.
```
$ git checkout abcde
Branch abcde set up to track remote branch abcde from origin.
Switched to a new branch 'abcde'
```

##### Sync up with remote and view current status of branches
```
$ git fetch --all; git branch -vv
* feature/pi-master 6ab71ca [origin/feature/pi-master] Added legacy pages for comparison tables
  master            4648ecb [origin/master] Merge feature/pi-master into master
Fetches latest changes to remote brances
List out your local branches with more information including what each branch is tracking and if your local branch is ahead, behind or both.
```

##### Fetch and merge
```
$ git pull - is the equivalent of git fetch && git merge.
```

##### Deleting remote branch
``` 
$ git push origin --delete abcde
To https://github.com/<project repo>
 - [abcde]         serverfix
```

### Prerequisites

What things you need to install the software and how to install them

```
Give examples
```

### Installing

A step by step series of examples that tell you how to get a development env running

Say what the step will be

```
Give the example
```

And repeat

```
until finished
```

End with an example of getting some data out of the system or using it for a little demo

## Running the tests

Explain how to run the automated tests for this system

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Deployment

Add additional notes about how to deploy this on a live system

## Built With

* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [Maven](https://maven.apache.org/) - Dependency Management
* [ROME](https://rometools.github.io/rome/) - Used to generate RSS Feeds

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 