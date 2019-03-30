# Contribution guidelines
Lysmarine have a github account for a  better reach out, but the actual work append on gitlab at
[https://gitlab.com/lysmarine](https://gitlab.com/lysmarine).


## Versioning & Branch
Pre-publishing work have been made in the `lysmarine` branch of `lysmarine-gen`

Now, Since version `0.8` workflow goes like this:  .
 - Development for the next version append on the `develop` branch.
 - Hot fixes append on a branch named `hotfix/[version number]`, then merged to `master` when ready.
 - Commits from upstream (pi-gen) are merged on the `develop` branch only.
 - Releases (including fixes) are merged to master and tagged with their version number.
 - The release images are compiled from `master` or `hotfix/` if needed.  


## Issues
If you work on lysmarine, you are invited to create a Issue to share your intent at [lysmarine-gen/issue](https://gitlab.com/lysmarine/lysmarine-gen/issue) .So others will see what you are working on.  

If you have found an issue or just something that don't feel right. Feel free to open an issue at [lysmarine/issue](https://gitlab.com/lysmarine/lysmarine/issue).


## Git

  If you work on a feature, it's best to do it on a separate branch forked from `develop` so the `PR` can be reviewed without preventing you to do some other works.(Or force lysmarine to accept multiples features/fix as a whole).

## Community guidelines
 * TODO *  But the basic apply, Be excellent to each others.
