**in master**
    git merge a_branch

CONFLICT (content): Merge conflict in conflict.txt
Automatic merge failed; fix conflicts and then commit.
    git status -s

UU conflict.txt

**we know the version of the file from the branch is the version we want.**
    git checkout --theirs conflict.txt
    git add conflict.txt
    git commit

# Sometimes during a merge you want to take a file from one side wholesale.
# The following aliases expose the ours and theirs commands which let you
# pick a file(s) from the current branch or the merged branch respectively.
#
# N.b. the function is there as hack to get $@ doing
# what you would expect it to as a shell user.
# Add the below to your .gitconfig for easy ours/theirs aliases.
#    ours   = "!f() { git checkout --ours $@ && git add $@; }; f"
#    theirs = "!f() { git checkout --theirs $@ && git add $@; }; f"
