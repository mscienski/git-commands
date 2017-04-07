**Delete local branches that have been merged into HEAD**
    git branch --merged | grep -v '\\*\\|master\\|develop' | xargs -n 1 git branch -d
**Delete local branches that have been merged into origin/master**
    git branch --merged origin/master | grep -v '\\*\\|master\\|develop' | xargs -n 1 git branch -d
**Show what local branches haven't been merged to HEAD**
    git branch --no-merged | grep -v '\\*\\|master\\|develop'
