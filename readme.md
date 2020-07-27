
# publishing reactjs app in github

1. Create repository in github

2. Goto local project directory and install gh-pages as given below

   npm install gh-pages --save-dev

3. in package.json, After private, create property homepage as given below

   "homepage":"http://<username>.github.io/repo name",

4. in package.json, after start, create following properties

   "predeploy": "npm run build",
   
   "deploy": "gh-pages -d build",

5. create local repository in the project directory

   git init

6. add the changes staneograpy area

   git add .

7.commit changes

   git commit -m "deploy"

8. remove previous remote repo origin

   git remote rm origin

9. add remote repo as origin

   git remote add origin https://github.com/mzndnes/mov.git

10. publish pages

   npm run deploy

