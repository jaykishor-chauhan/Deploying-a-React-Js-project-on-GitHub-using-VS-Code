# Deploying-a-React-Js-project-on-GitHub-using-VS-Code


## 1. Installing Git in your system

#### 1.1 Click on `Download Git` to download the Git on your system. if you have already downloaded ignore it.
#### [Download Git](https://git-scm.com/downloads) 

#### 1.2 After downloading, Install `Git` in your system.

#### 1.3 Set Up Git in VS Code
#### Ensure Git is installed and configured on your system to chack git version. <br />
      git --version


## 2. Initialize Your Project
#### Open the project folder in VS Code. and Initialize Git in the project folder:
    git init

## 3. Install gh-pages 
#### GitHub Pages is a free service provided by GitHub that allows you to host static websites directly from your repository:
    npm install gh-pages --save-dev

## 4. Stage and Commit Changes
#### Use the Source Control tab in VS Code or terminal commands:
    git add .
    git commit -m "Initial commit"

## 5. Connect to GitHub Repository
#### Link your local project to the GitHub repository:
    git remote add origin <repository-URL>
##### replace "repository-URL" with your own "repository-URL"

## 6. Push to GitHub
#### Push your changes to the main branch:
    git branch -M main
    git push -u origin main

# 7. Now, modify your package .json files by adding key-value pair mentioned below or You can refer to the images:
#### (1) open package.json file and add homepage befor name:
        "homepage":"http://(GitHub user name).github.io/(repo. name)"
        
##### [(replace GitHub user name with your own GitHub user name and repo. name with your Repository name.)]
#### (2) update script:
        "predeploy": "npm run build",
        "deploy": "gh-pages -d build"

![Image Description](https://drive.google.com/uc?export=view&id=1wmkk1M0IXOpBV_Fb8nDECimmnLGEwaJI)


## And finally, built and deploy your project using:
    npm run build
    npm run deploy 
