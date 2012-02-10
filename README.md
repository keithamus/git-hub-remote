This is a quick bash script to create a git repository on your github account, 
while also adding it to your remote.

Setup:

    cp git-hub-remote /usr/local/bin/git-hub-remote
    git config --global github.username my_github_username
    git config --global github.token my_github_api_token


Usage:

    git hub-remote reponame
    # Creates PUBLIC repo "reponame" under your user, and adds "github.com/user/reponame" as "origin" remote

    git hub-remote reponame upstream
    # Creates PUBLIC repo "reponame" under your user, and adds "github.com/user/reponame" as "upstream" remote

    git hub-remote --private reponame
    # Creates PRIVATE repo "reponame" under your user, and adds "github.com/user/reponame" as "origin" remote
