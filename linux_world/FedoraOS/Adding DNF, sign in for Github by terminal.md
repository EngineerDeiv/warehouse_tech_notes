1. Add this repo
~~~
sudo dnf config-manager addrepo --from-repofile=https://cli.github.com/packages/rpm/gh-cli.repo
~~~
2.  run this command for installs gh login 
~~~
sudo dnf install gh
~~~
3. verified the version of gh
~~~
gh --version
~~~ 
4. do login
~~~
gh auth login
~~~

