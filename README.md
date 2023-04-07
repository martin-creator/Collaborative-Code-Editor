# Collaborative Code Editor(CCE)
![Imgur](https://i.imgur.com/OxrG6hm.jpg)

## Introduction

[Live Demo]( https://collaborartive-code-editor.onrender.com/)

Many collaborative code editors with essential features like video chats come at a relatively high price for developers from underdeveloped countries, making coding with friends/family impossible. 

This collaborative code editor provides individuals and businesses with the infrastructure to simplify real-time remote pair programming.  

> CCE aims to allow every software developer to pair-program at no cost!

![Imgur](https://i.imgur.com/duJX0nw.jpg)

## Purpose
According to the [Stackoverflow developers’ survey of 2022](https://survey.stackoverflow.co/2022/), out of the 70,000 survey participants, only 3.3% are African, and 1.48% are Black. This statistic accurately captures the dire need to increase the developer population in Africa to support the digital transformation of our sectors so that we can provide services to the people most in need. According to the [2020 Google economy report](https://innovationvillage.co.ug/wp-content/uploads/2021/12/Final-DevScape-Report-2021-compressed-1_1.pdf), there are 11,000 developers in Uganda serving a population of 44.7 million people,  which is a low number if our tech ecosystem is to compete in Africa. 

Many companies and organizations like [ALX Africa](https://www.alxafrica.com/), [Andela](https://andela.com/), [Tunga](https://tunga.io/) have come up with programs to train Africans in the latest development technologies to bridge this gap. One of the challenges faced during software development programs is the lack of structured mentorship. Ideally, when a student needs help to understand a particular algorithm, the only tools available are zoom or google meet, which do not support real-time code collaboration, thus making the mentor-students session less interactive. 

To address, the problem of non-interactive coding sessions between mentors and students in African software development training programs, I decided to build **CCE** to  enable students and mentors to: 

* conduct real-time, remote **pair programming** sessions
* conduct real-time, remote **tutoring** sessions
* conduct real-time, remote **mock coding interviews**


**CCE's** video conferencing and chat features ensure that the coding sessions are interactive as possible.

## Tech Stack(Dependencies)

### 1. Backend Dependencies
Our tech stack includes the following:
* [**Node.js**](https://nodejs.org/en/) server side platform
* [**Express.js**](http://expressjs.com/) web framework
* [**Socket.io**](https://socket.io/) for real-time webpage updates
* [**Passport.js**](http://www.passportjs.org/) authentication
* [**MongoDB**](https://www.mongodb.com/what-is-mongodb) NoSQL database
* [**Mongoose**](http://mongoosejs.com/) Object-relational mapper

### 2. Frontend Dependencies
You must have the **HTML**, **CSS**, and **Javascript** with [Bootstrap 3](https://getbootstrap.com/docs/3.4/customize/) for our website's frontend.  Our Websites frontend has been installed using [bootstrap cdnjs](https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/3.3.7/js/bootstrap.min.js). 

Our tech stack includes the following:
* [Handlebars](http://handlebarsjs.com/) HTML templating language
* [Bootstrap3](https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/3.3.7/js/bootstrap.min.js) ready-to-use HTML and CSS component kit

## Prerequisites
- Install a [Node Version Manager (NVM)](https://github.com/creationix/nvm)
- Download and install Node.js from [here](https://nodejs.org/en/)
- Alternatively, you can download and install Node.js using the [node version manager](https://github.com/nvm-sh/nvm) ```$ nvm install @latest version of node``` 
- Install [MongoDB](https://www.mongodb.com/) by following the instruction in this [document](https://docs.microsoft.com/en-us/windows/wsl/tutorials/wsl-database) if you are using windows. 
- Download studio 3T and install [Studio 3T](https://studio3t.com/) GUI for exploring the database content. This makes managing your local database very easy.
- Open now the  application, and create a MongoDB database. Enter your database configuration settings under ```config.js:11```.

## Customization

### Modifying Local Files
- Configure the  mailer servicenunder ```config.js```
- Replace the ```dbConnString``` inside the ```config.js:12```. It should be similar to e.g. ```mongodb://<dbuser>:<dbpassword>@abc12345.mlab.com:21336/codasession```.
- To implement the github login strategy, replace the following cotents in passport js:43 
``` 
{
    clientID: ****,
    clientSecret: *****,
    callbackURL: ***,
} 

```

### Modifying the frontend
-We have only implementend basic designs for our html pages, feel free to customize the html to meet your design needs.  

## Running the App Locally
- Run ```$ npm install``` to install all dependencies
- Run ```$ npm start``` to start the web server
- Run ```$ sudo mongod``` to start the NoSQL database
- Your local machine: Open your web browser and go to ```localhost:3000```.


## Deployment

### Going Online
- Choose any cloud hosting service like [Amazon Web Services](https://aws.amazon.com/s3/), [Google Cloud](https://cloud.google.com/), [Azure](https://www.azure.microsoft.com/) to deploy your application. 
**Please remember to check the cloud providers documenation on specific instructions on the deployment process**

## Support
If you encounter any challenges while installing this application, please don't hesitate to shoot me an email to <martinlubowa@outlook.com>

## Check out these resourses to learn about operational transformation, the technology behind collaborative code/text editors. 

* [Operational Transformation, Wikipedia](https://www.google.com/search?q=operation+transformation&oq=operation+trans&aqs=chrome.0.0i355i512j46i512j0i512j69i57j0i512j69i60l3.18079j0j4&sourceid=chrome&ie=UTF-8)
* [Operational Transformation JS](https://github.com/Operational-Transformation/ot.js/)

