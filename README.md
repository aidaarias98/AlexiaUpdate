## ![ally](https://user-images.githubusercontent.com/112099409/216687498-0c6a30db-6794-4976-a95c-cc749867bc8a.png)- Capstone Project

Mentally is a react application 

## Features
- Home
- MyHealth360
- Motherhood360
- MyMind360
- Contact
- Chat
- Sign Up / Log In

## Using and Running our app
In order to begin using our app.....
Download the app to your local machine. Delete all the "package-lock.json" files. Next, open a terminal and go to the api directory(cd api) and do a npm install. Open another terminal and go to the client directory (cd client) and do a npm install. 

To get the app running 
You will open a terminal for your api (cd api) and then npm start. And open another terminal for your client folder (cd client) and do another npm start. If you accidently kill ther terminal this is how you would get the app up and running again.


To get conneted with the mysql database you are going to go in the "api" folder and go to the "db.js" file and change the mysql info to your personal info

Here are the queries used for the creation of the database:

CREATE DATABASE blog;
USE blog;
CREATE TABLE users (
  id INT NOT NULL AUTO_INCREMENT PRIMARY KEY,
  username VARCHAR(255),
  email VARCHAR(255),
  password VARCHAR(255)
);
CREATE TABLE contactData(
id INT AUTO_INCREMENT PRIMARY KEY,
fullName VARCHAR(255),
email VARCHAR(255),
message VARCHAR(255)
);
CREATE TABLE messages(
messageId INT AUTO_INCREMENT PRIMARY KEY,
senderID INT,
recipientID INT,
message VARCHAR(255),
chatID INT,
date DATETIME
);
CREATE TABLE chat(
id INT,
flag ENUM('open','close')
);
CREATE TABLE mentalFormAnswers(
id INT,
fullName VARCHAR(45),
q1 VARCHAR(45),
q2 VARCHAR(45),
q3 VARCHAR(45),
q4 VARCHAR(45),
q5 VARCHAR(45),
q6 VARCHAR(45),
q7 VARCHAR(45),
q8 VARCHAR(45),
q9 VARCHAR(45),
q10 VARCHAR(45)
);

## Stopping the app
To Stop the app from working all you wanna do is either kill the terminal or open a terminal for your client folder (cd client) and in the terminal you can do "ctrl" and "C" at the same time on your keyboard to stop the react app from running.

## Created with:
- React: Framework used
- Node.js: Utilize to create server
- Javascript
- Tailwind
- Express.js - Used for routes and endpoints
- Cors
- Axios
- MySQL 2
- MySQL
- BcryptjS
- Cookie-parser
- Jsonwebtoken
- Multer
- Nodemon
- Socket.io

## Authors
- Alexia Lorenzana
- Aida Arias
- Y-Jacob Mlo
- Alannah Gregory
- Said Guzman Zaragoza
- Sheldon Ferguson
