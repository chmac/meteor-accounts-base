meteor-accounts-base
====================

Fork of accounts-base including a simpler version of meteor/meteor#1845

To update this, do the following:

cd /path/to/meteor
git checkout devel
git pull
git checkout release/0.X
git subtree split -P packages/accounts-base -b accounts-base-only
cd /path/to/accounts-base-only/
git pull /path/to/meteor accounts-base-only
git push

Note, the module might not be updated properly, solution was:

```
cd ~/.meteorite/source/git@github.com\:chmac/meteor-accounts-base/
git pull
```
