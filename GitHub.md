# GitHub 

## Authentication error when pushing to wiki repos

Wiki git repo URLs on GitHub are not SSH based, so you need to adapt them in order to push (in some circumstances):
`https://github.com/haroon/something.wiki.git` > `git@github.com:haroon/something.wiki.git`
