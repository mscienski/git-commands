**Made lots of local commits and haven't run any tests...**
    [unittest runner of choice]
**Failures... now unclear where it was broken.**

**git bisect to rescue.**
    git bisect start # to initiate a bisect
    git bisect bad   # to tell bisect that the current rev is the first spot you know was broken.
    git bisect good <some tag or rev that you knew was working>
    git bisect run [unittest runner of choice]
**Some runs.**
**BLAMO -- git shows you the commit that broke**
    git bisect reset
**to exit and put code back to state before**
    git bisect start
**Fix code. Run tests. Commit working code. Make the world a better place.**
