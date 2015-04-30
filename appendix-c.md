# Appendix C: Deploy on the web

In this workshop, you developed your web service on the local machine (i.e. http://localhost/) which means that only yourself and people 
on the same network can eventually access your web site using your ip address.

For example, you can use http://localhost/ or http://127.0.0.1/ to access your machine web site (127.0.0.1 is the default address for your network card),
and other people should use the real ip address instead (usually something like http://192.168.1.55/). Running a web site on the local machine is only 
required for development purprose, but you may want to make the web site available to anyone in the world. To do this you need to deploy your web site 
on a web server.

A very easy way to do this is to use ['heroku'](https://www.heroku.com/) which has a nice feature to a web site deploy from github.

<b>Step 1</b> Sign up on [herokuc.com](https://www.heroku.com/) for a free account

<b>Step 2</b> Create a node.js server by selecting the '+' sign on the top-right corner

 ![](img/heroku-createserver.png)
 
<b>Step 3</b> Push the 'Create App' button. You can leave the name field empty, and use the location you prefer.

 ![](img/heroku-createapp.png)
 
<b>Step 4</b> By default, heroku will show the 'Deploy' page, if not, select 'Deploy'

 ![](img/heroku-deploy.png)
 
<b>Step 5</b> Next, select 'GitHub - Connect to GitHub'

 ![](img/heroku-github.png)

<b>Step 6</b> Next, Press 'Connect to GitHub'

 ![](img/heroku-connect.png)

<b>Step 7</b> Search for your repo

 ![](img/heroku-search.png)

<b>Step 8</b> When your repo was found, press the connect button

 ![](img/heroku-github-connect.png)

<b>Step 8</b> Finally, choose the branch you want to auto-deploy (usually master), and press the 'Enable Automatic Deploys' button.

 ![](img/heroku-auto-deploy.png)

 Now, heroku should show the following when you'll come back on your server dashboard.
 
 ![](img/heroku-results.png)
 
 Whenever you will push a change on github, the site will be rebuilt with the source found on your GitHub repository.
 
<b>Note</b> You can still deploy manually if you want, by pressing the 'Deploy Branch' button at the bottom of the page. 
This is actually needed for the first time unless you push a change on github.

<b>Note</b> On the 'Activity' tab, you can see when and if your site was rebuilt successfully or not.


=========================  
[Home](README.md)