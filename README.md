# amend-merge-commit

I am curious to see what happens when I amend a merge commit. I do it now on purpose, but I have seen it also done accidentally. 
Right now I see no easy way to tell what happened to a merge commit.

Story:

 - File `a2.txt` is added to the `master` branch. (https://github.com/csabakoncz/amend-merge-commit/commit/3896860ac23cf2a79af66b2b1c5a538d0861d20f)
 - branch `b` merges the master branch and then amends the merge commit so that `a2.txt` is deleted. (https://github.com/csabakoncz/amend-merge-commit/commit/943854e1c0e6d9f42b7ce7f6368e7d19ca21816d) The log says there are no changes!
 - `b` is merged into `master`. `a2.txt` disappeared, but `git log` does not tell you where.
