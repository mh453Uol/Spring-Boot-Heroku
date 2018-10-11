# Spring-Boot-Heroku
Deploying Spring Boot Apps to Heroku For Free Guide 

Before getting starting with deployment we need to do 2 things;

1. Create an account on Heroku - https://signup.heroku.com/ enter email, name etc..
2. Download the Heroku CLI - https://devcenter.heroku.com/articles/heroku-cli we are going to use the command line interface to upload our project to heroku. 

Here we go

For this guide we are going to create the simpliest spring application possible.

1. Go to https://start.spring.io/ 
2. (Important) under packaging (click Switch to the full version) make sure you select jar and have web and rest rest repositories selected under dependencies. 
3. Click generate project
4. Now the project is downloaded, unzip the project. 
5. Open the cmd
6. Navigate to your project
7. Inside the src/main/resources/static add your html, minified angular app or react app here.
8. If you added files to the static folder you can check they work by running the spring boot app locally. 
9. Inside the console enter heroku login and enter your credentials. When I first tried this it didnt work however I opened the cmd as admin and it worked fine.
10. Enter git init
11. Enter git add .
12. Enter git commit -m "first commit"
13. Enter heroku create - This create a new Heroku app project and give it a random url. Output would look like Creating nameless-lake-8055 in organization heroku... done, stack is cedar-14
http://nameless-lake-8055.herokuapp.com/ | git@heroku.com:nameless-lake-8055.git
Git remote heroku added
14. Enter git push heroku master to deploy your app
15. heroku open to open your web app in the browser
16. You can rename your application by entering heroku apps:rename xyz

Good docs 
https://devcenter.heroku.com/articles/deploying-spring-boot-apps-to-heroku
https://www.callicoder.com/deploy-host-spring-boot-apps-on-heroku/

Thanks ;)


