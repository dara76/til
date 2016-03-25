### Searching all my commits in all my branches for some text

    git rev-list --all | xargs git grep <regexp>

    git rev-list --all -- <path> | xargs git grep <regexp>


http://stackoverflow.com/questions/2928584/how-to-grep-search-committed-code-in-the-git-history#2929502
