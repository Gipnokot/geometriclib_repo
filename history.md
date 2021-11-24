git clone https://github.com/smartiqaorg/geometric_lib
cd geometric_lib
git checkout develop
git log --all --pretty=oneline --graph
git checkout future
git log --all --pretty=oneline --graph
git checkout main
git merge --no-ff develop
git log
git revert HEAD~1 -m 1
git checkout release
git rebase main
git log
git checkout main
git merge release
git push geom main
