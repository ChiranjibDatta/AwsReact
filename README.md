# Practice how to deploy react app using AWS AMplicy and CI/CD.
**The below documentation may be changed as per the AWS latest documentation. The idea of the project is to showcase how quickly a react APP can be hosted into AWS. If the below steps does not work please check the AWS documentation**

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).
 <br /><br />
 **Step1**: Create a Reat project using [create-react-app](https://create-react-app.dev/)
 <br /><br />
 
 **Step2**: In this step, you will create a GitHub repository and commit your code to the repository. You will need a GitHub account to complete this step—if you do not have an account, sign up here.
<br/><br/>

a. Create a new [GitHub repo](https://github.com/new) for your app
<br/><br/>
![Github](https://d1.awsstatic.com/webteam/getting_started/GSRC%202020%20updates/Front%20End/Front%20End%20GitHub%20Repository%20Module%201.200d68b2582dc550603aeb4111fbf9c29cca8669.png)
<br/><br/>

b. Using create-react-app will automatically initialize the git repo and make an initial commit. If you are trying to deploy an existing React application where git has not been initialized, make sure to input the following commands before continuing:
<br/><br/>

````
git init
git add .
git commit -m "initial commit"
````
<br/><br/>

c. Push the application to the new GitHub repo by executing the following commands in your command line interface:
<br/><br/>
````
git remote add origin git@github.com:username/reponame.git
git branch -M main
git push -u origin main
````
<br/><br/>

**Step3**: Login to AWS Managemen console. Create an account using your credit card. (You will not be charged untill and unless you are using anything other than free tier)
<br><br/>
Open the AWS Management Console in a new browser window, so you can keep this step-by-step guide open. When the screen loads, enter your user name and password to get started. Then enter Amplify in the search bar and select AWS Amplify to open the service console.
![AWS](https://d1.awsstatic.com/webteam/getting_started/GSRC%202020%20updates/Front%20End/Front%20End%20AWS%20Console%20Find%20Amplify%20Module%201.7f67ad70cf09eddb21a035ac263a2eb0a7e88df5.png)
<br><br/>

**Step4**: Deploy your app with aws amplify
<br><br/>
In this step, you will connect the GitHub repository you just created to the AWS Amplify service. This will enable you to build, deploy, and host your app on AWS.
<br><br/>
a. In the AWS Amplify service console, select Get Started under Amplify Hosting.
<br/><br/>
![AWS1](https://d1.awsstatic.com/webteam/getting_started/GSRC%202020%20updates/Front%20End/Front%20End%20Amplify%20Deploy%20Module%201.ac4bb6b718f3e6550f8aaa23c85c3a1dd6359a1b.png)
<br/><br/>

b. Select GitHub as the repository service and select Continue.
<br/><br/>
![AWS1](https://d1.awsstatic.com/webteam/getting_started/GSRC%202020%20updates/Front%20End/Front%20End%20Amplify%20GitHub%20Module%201.dabc4acb9a363d29d13bfdd20b1ccd880510edb0.png)
<br/><br/>

c. Authenticate with GitHub and return to the Amplify console. Choose the repository and main branch you created earlier, then select Next.
<br/><br/>
![AWS1](https://d1.awsstatic.com/webteam/getting_started/GSRC%202020%20updates/Front%20End/Front%20End%20GitHub%20Add%20Repository%20Module%201.e1bd69f42d47cc002b3c785f0c91563058fd0650.png)
<br/><br/>

d. Accept the default build settings and select Next.
<br/><br/>
![AWS3](https://d1.awsstatic.com/webteam/getting_started/GSRC%202020%20updates/Front%20End/Front%20End%20GitHub%20Add%20Repository2%20Module%201.0a77c277aa92d616fe8728f1a1a761203153e654.png)
<br/><br/>

e. Review the final details and choose Save and deploy.
<br/><br/>
![AWS4](https://d1.awsstatic.com/webteam/getting_started/GSRC%202020%20updates/Front%20End/Front%20End%20GitHub%20Add%20Repository3%20Module%201.37a6eae83a1a152d9bf5c7fc11b767ada1cee761.png)
<br/><br/>

f. AWS Amplify will now build your source code and deploy your app at https://...amplifyapp.com.
<br/><br/>
![AWS5](https://d1.awsstatic.com/webteam/getting_started/GSRC%202020%20updates/Front%20End/Front%20End%20Amplify%20Deploy%20Source%20Module%201.5f5bddd11232f278092ad790fa67066ac9c96ea6.png)
<br/><br/>

g. Once the build completes, select the thumbnail to see your web app up and running live. 
<br/><br/>
![AWS6](https://d1.awsstatic.com/webteam/getting_started/GSRC%202020%20updates/Front%20End/Front%20End%20Initial%20App%20Module%201.ba286128748534afaa9769ca76675680a4e13047.png)

<br/><br/>


**Step4**: Automate pipeline and deploy your code changes. Do some changes in the code and push to your git repository
<br/><br/>
```
git add .
git commit -m “changes for v2”
git push origin main
```
