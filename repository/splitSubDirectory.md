    $ git clone ssh://stash/proj/mcplugins.git
    $ cd mcplugins
    $ git checkout origin/master -b mylib
    $ git filter-branch --prune-empty --subdirectory-filter plugins/mylib mylib
    $ git push ssh://stash/proj/mylib.git mylib:master
