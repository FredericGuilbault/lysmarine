# Contribution guidelines
Lysmarine have a github account for a  better reach out, but the actual work append on gitlab at
[https://gitlab.com/lysmarine](https://gitlab.com/lysmarine).

Most of lysmarine is created in the [lysmarine-gen](https://gitlab.com/lysmarine/lysmarine-gen) repository.

## Versioning & Branch
Pre-publishing work have been made in the `lysmarine` branch of `lysmarine-gen`

Now, Since version 0.8 workflow goes like this:  .
 - Development for the next version append on `develop` branch.
 - Hot fixes append on a branch named from the version number, then merged to `master` when ready.
 - Commits from upstream append on the `develop` branch only.
 - Releases (including fixes) are tagged with their version number.
 - The release images are compiled from `master`.  


## Issues
If you work on lysmarine, you should create a Issue to state your intent at [lysmarine-gen/issue](https://gitlab.com/lysmarine/lysmarine-gen/issue) .So others will see what you are working on.  

If you have found an issue or just something that don't feel right. Feel free to open an issue at [lysmarine/issue](https://gitlab.com/lysmarine/lysmarine/issue).


## Git

  If you work on a feature, it's best to do it on a separate branch forked from `develop` so the `PR` can be reviewed without preventing you to do some other works.(Or force lysmarine to accept multiples features/fix as a whole).

## Community guidelines
TODO. But the basic apply, Be excellent to each others.
