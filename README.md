# Project Title

One Paragraph of project description goes here

## Cheatsheet

```
git remote show origin
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

In scenario below.
* Add + commit file to testing branch. Switched to master.
* Add + commit file to master branch. Switched to develop.
* Add/modify + commit file to develop and ran git log command to see current state.
```
git log --oneline --decorate --graph --all
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

## Authors

* **Billie Thompson** - *Initial work* - [PurpleBooth](https://github.com/PurpleBooth)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc
