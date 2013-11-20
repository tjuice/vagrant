vagrant
=======

 Clone REPOSITORY

# In this example, we use an external account named extuser and
# a GitHub account named ghuser to transfer repo.git

git clone --bare https://githost.org/extuser/repo.git
# Make a bare clone of the external repository to a local directory

cd repo.git
git push --mirror https://github.com/ghuser/repo.git
# Push mirror to new GitHub repository

cd ..
rm -rf repo.git
# Remove temporary local repository
