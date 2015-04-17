# git-whereami
*Append your location to all of our git commits!*

Do you travel a lot?  Would you team be interesetd to know where your code is coming from?  Then this is for you!

1. Install `whereami`
  - Head on over to https://github.com/robmathers/WhereAmI and download the `whereami` excecutable. Place it in your home folder, like `~/whereami`

2. In whichever git repository you want to use this on, copy the `prepare-commit-msg` into `~/PROJECT/.git/hooks`.

**That's it!**

Now, whenever you make a `git commit`, we will use `whereami` to source yoru lat/lng, and then ask Google's geocoder what your address is, resulting in:

```bash

# Please enter the commit message for your changes. Lines starting
# with '#' will be ignored, and an empty message aborts the commit.
# On branch master
# Your branch is ahead of 'origin/master' by 4 commits.
#   (use "git push" to publish your local commits)
#
# Changes to be committed:
#       new file:   newfile
#

This commit coded at:
---------------------
63 Hanbury Street London E1 5JP UK
51.520182, -0.070440
@ Fri Apr 17 15:57:03 BST 2015
```

Feel free to tweak the template as you wish!

---

## Notes:

- OSX Only!
