### Version control systems

#### Centralized version control systems
Centralized vcs's are based on the idea that there is a single "central" copy of your project somewhere (probably on a server), and programmers will commit their changes to this central copy.

#### Distributed version control systems
Distributed vcs's do not necessarily rely on a central server to store all the versions of a projects file, every developer "clones" a copy of a repository and has the full history of the project on their own hard drive.

##### Pros:
* Actions other than pulling and pushing is extremely fast because the tools needs access to the hard drive, and not a remote server
* Committing new change sets can be done locally without anyone else seeing them. Once you have a group of change sets ready, you can push all of them at once
* Everything except push/pull can be done without internet access
* Easy reviewing others changes since each programmer has a full copy of the repository
