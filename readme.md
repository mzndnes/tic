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
   
# remove previous remote origin as given below
5. git remote rm origin

#add remote origin
6. git remote add origin https://github.com/mzndnes/mov.git

#publish pages
7. npm run deploy
