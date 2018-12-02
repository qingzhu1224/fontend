git checkout --orphan gh-pages
git rm --cached -r .
git clean -df
rm -rf *~


echo "*~" > .gitignore
echo "_book" >> .gitignore
git add .gitignore
git commit -m "Ignore some files"