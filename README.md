[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/9NDadFFr)
Add design docs in *images/*

## Instructions to setup and run project
- Setup mongoDB community edition
  - from https://docs.mongodb.com/manual/administration/install-community/
  - start it as a background service. MongoDB service will run on 127.0.0.1 (localhost), port 27017.
- Libraries for Client
  - npm install axios
- Libraries for Server
  - npm install express
  - npm install mongoose
  - npm install cors
  - npm install bcrypt
  - npm install express-session
  - npm install -g nodemon
- After installing all necessities
  - cd into server and run node init.js (username) (password)
  - ex: node init.js admin 123456
  - email used for login can be found in init.js for admin login and other accounts
  - npm start in client directory to start react and nodemon server.js in server directory to start server

## Team Member 1 Contribution (Allen Lin)
- Created login page + CSS
- Created register page + CSS
- Created welcome page + CSS
- Created schema for accounts
- Questions
    - made question summary
    - updated it to 50 characters
    - added votes and summary to schema 
- Created Profile page + CSS
    - added username
    - added reputation
    - added questions asked
    - added questions answered
    - added tags
    - created admin with the ability to delete users
- Server 
    - added routes for login, register, and welcome
    - added routes for questions
    - added routes for profile
        - updating the other parts of the database such as other user's answers and questions
    - added routes for admin
        - deleting users
- init
    - created the presets for the database
- Testing
    - tested the cases from the documentations
    - fixed bugs and stressed tested the website
- Created the UML diagram

## Team Member 2 Contribution (Shawn Zhu)
- Client
  - Main
    - header
      - used code from hw3
      - added Vew profile to click to view profile
    - leftnav
      - used code from hw3
      - added logout and signin/up button and their mechanism 
    - rightcontent
      - used code from hw3
      - added edittag and prodfile component
    - login
      - created handlesubmit for user login
    - signup
      - created handlesubmit for sign up
    - welcome
      - verify if there is a session to maintain logged in
  - Pages
    - askquestion
      - used code from hw3
      - modified to allow edit question and delete question when edited from profile page
    - home
      - used code from hw3
      - modified so only 5 questions are shown at a time and have two buttons to navigate them
    - tags
      - used code from hw3
    - edittag
      - allow edit and delete one tag
    - profile
      - made all edit functions, tag delete function
      - allow admin to view and modify users profile, admin can go back to their own profile,
      - added display no question/answer/tags
  - fakestackoverflow
    - used code from hw3
    - added welcome, signup, login component
- Server
  - server
    - made some of the methods
  - model
    - made new model for comment
    - modified other models by adding new fields
  - init
    - revised to maek sure no error
- Other
  - handled system/communication failed with error messages
