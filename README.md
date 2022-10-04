#OurMap

OurMap is an interactive map where users can set pin on locations of their interest, leaving reviews, comments, or summaries about places they have been to.

##Local Installation
##Frontend
Starting at the project's root:
```
cd frontend
npm install yarn
npm install react-scripts
```
To run the project:
```
yarn start
```
##Backend
Starting at the project's root:
```
npm install yarn
npm install react-scripts
```
To run the project:
```
yarn start
```


##Pin Types
###Local Radius
OurMap defines the locality radius as the radius of Tokyo, Japan, due to it being considered the largest city in the world.
###Local
A pin type is considered local if it's within the locality radius relative to the user's home location.
###Tourist
A pin type is considered a tourist pin if it's outside of the locality radius relative to the user's home location.

##Front End and Back End
This repository contains the front end of the app, where we interact with the user, draw the map, and allow the user to create pins. The [back end can be found here](https://github.com/tydan3/OurMap_Backend).

##CI/CD Pipeline
![image](https://user-images.githubusercontent.com/34032935/193659142-686413f0-91d4-48f5-a3f2-985b8b82583b.png)
