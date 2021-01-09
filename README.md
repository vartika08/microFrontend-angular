This github repository has four projects all in one repo. But when you do this yourself, you'll want to have one git repo per angular application. 
The root-html-file project should also be in its own repo. This is what lets different teams and developers be in charge of different microfrontends.

With single-spa, it is preferred to run ng serve in only one single-spa application at a time, while using a deployed version of the other applications. This makes for an awesome developer experience where you can boot up just one microfrontend at a time, not even having to clone, npm install, or boot up all of the other ones.

To try this out, clone the repo and run the following commands:

# Local development -- one app at a time

cd app1
npm i
npm start

# Local development -- all at once

It is preferred to only run one app at a time. But if you need to run them all locally, you can do so with the following instructions

* First terminal tab =>
cd root-html-file >
npm install >
npm start

* Second terminal tab =>
cd app1 >
npm install >
npm start

* Third terminal tab =>
cd app2 >
npm install >
npm start

* Fourth terminal tab
cd navbar
npm install
npm start
Now go to http://localhost:4200 in a browser. 

Note that you can change any of the ports for the projects by modifying the Import Map inside of root-html-file/index.html.
