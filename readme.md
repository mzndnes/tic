# tic
# publishing reactjs app in github

1. Create repository in github

# Goto local project directory and install gh-pages as given below
2. npm install gh-pages --save-dev

# in package.json, After private, create property homepage as given below
3. "homepage":"http://<username>.github.io/repo name",

# in package.json, after start, create following properties

4. "predeploy": "npm run build",
   "deploy": "gh-pages -d build",

5. git init

# add the changes
6. git add .

# commit changes
7. git commit -m "deploy"

# remove previous remote origin as given below
8. git remote rm origin

#add remote origin
9. git remote add origin https://github.com/mzndnes/mov.git

#publish pages
10. npm run deploy

# clone the remote repoitory to local
git clone https/github.com/mzndnes/pra.git

# push to cloned remote repository
git push origin master

# check the clone url
git remote -v
