# first: stage the changes you want incorporated in the previous commit

# use -C to reuse the previous commit message in the HEAD
$ git commit --amend -C HEAD
# or use -m to make a new message
$ git commit --amend -m 'add some stuff and the other stuff i forgot before'
