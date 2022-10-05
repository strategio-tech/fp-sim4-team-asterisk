# OurMaps

<img width="1396" alt="Screen Shot 2022-10-05 at 11 59 15 AM" src="https://user-images.githubusercontent.com/61354783/194106958-9e2ca627-b78d-487f-8192-2988958f16ba.png">

OurMaps is an interactive map where users can set pin on locations of their interest, leaving reviews, comments, or summaries about places they have been to.

## Table of Contents
- [Background](#background)
- [Pin Types](#pin-types)
- [Functionalities](#functionalities)
- [Front End and Back End](#front-end-and-back-end)
- [CI/CD Pipeline](#cicd-pipeline)
- [Local Installation](#local-installation)

## Background

OurMaps is built upon a member's previous work and is currently a working Final Project by Team Asterisk from the Strategio Enterprise Simulator. This goal of this project is to create and integrate a CI/CD pipeline into a web application.

## Pin Types
**_Note:_** OurMaps defines the locality radius as the radius of Tokyo, Japan, due to it being considered the largest city in the world.
### Local
A pin type is considered local if it's within the locality radius relative to the user's home location.
### Tourist
A pin type is considered a tourist pin if it's outside of the locality radius relative to the user's home location.

## Functionalities

### Register an account
![image](https://user-images.githubusercontent.com/61354783/194100514-f06e0778-0777-4421-8d8f-f8f7f1d2addf.png)

Username and password are case sensitive.

### Sign in
![image](https://user-images.githubusercontent.com/61354783/194100565-d50f4c88-804f-42a3-aa30-c4b2ad6665ac.png)

Sign in with your registered account. Pins associated to your account will be in red. For demonstration purposes, you may also use the test account

Username: anon <br />
Password: anon123?

### Create a pin
![image](https://user-images.githubusercontent.com/61354783/194098698-7cc82336-fe69-4969-8032-e578b3e3c08e.png)

Create a pin by double-clicking and fill in the fields to leave a review.

### Delete a pin
![image](https://user-images.githubusercontent.com/61354783/194100180-ebc409aa-e20b-4119-9521-a5b555c24e42.png)

You may only delete pins that are associated with your account. To delete a pin, select your pin and click the delete button ini the pin's info window.

### How To
<img width="229" alt="Screen Shot 2022-10-05 at 11 57 31 AM" src="https://user-images.githubusercontent.com/61354783/194106635-2df429bb-1736-49d0-8dee-046373c62d56.png">

More in depth instructions can also be found with the How to Use button found in the navigation bar of the site.

## Front End and Back End
This repository contains the front end of the app, where we interact with the user, draw the map, and allow the user to create pins. The backend repository is added as a submodule. For more information on how to use submodules, please refer to this [link](https://github.blog/2016-02-01-working-with-submodules/).

## CI/CD Pipeline
![image](https://user-images.githubusercontent.com/34032935/193659142-686413f0-91d4-48f5-a3f2-985b8b82583b.png)

## Local Installation

First clone the repository and cd into the appropriate directory to run the installation commands.

### Frontend
Starting at the project's root directory:
```
cd OurMap/OurMap_frontend/frontend/
npm install yarn
npm install react-scripts
```
To run the project:
```
yarn start
```

**_Note:_**  if `yarn start` does not work, you can also run the project by using `npm start`.

### Backend
Starting at the project's root directory:
```
cd OurMap/backend
npm install yarn
npm install react-scripts
```
To run the project:
```
yarn start
```

**_Note:_**  if `yarn start` does not work, you can also run the project by using `node server.js`.

## Local Deployment
In order to make this run purely on the local machine, there are some changes in the code to make. Within the frontend folder, there are three files to change the code: App.js, Register.jsx, and Signin.jsx.

Replace all instances of https://ourmapserver.click with http://localhost:8800 in the following places: <br />
- App.js, line 13
- Register.jsx, line 25
- Signin.jsx, line 25

You will then be able to open the project with the link http://localhost:3000 when running the project in development mode with `yarn start`.