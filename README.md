# Oboardgame

Oboardgame is a collaborative project, developped during the last month of class in O'clock virtual school (https://www.oclock.io).

The team :
+ [Mathis Pati](https://github.com/Mathis-web), Product Owner & Backend Developper
+ [Killian Courvoisier](https://github.com/KillianCourvoisier), Lead Backend Developper
+ [Osée Ralantoarison](https://github.com/oralanto), Lead Frontend Developper
+ [Kaio Fernandes Dias Cordeiro](https://github.com/KaioFernandes), Git Master & Frontend Developper
+ Cédric Leizour (myself), Scrum Master & Frontend Developper

_____________________________________________________________

## **The Project**

We notice that usually, boardgames are pretty expensive, and often, we hesitate buying them because of the potential lack of interest afterward. Then we came with Oboardgame, a (future) web application where you can rent boardgames of any type, for cheap, for the week or a few days.

The concept here is to be able to post, update, and rent with small ads and small wallets from your favourite boardgames experiences. Be able to share, the great moment you had playing this mighty Risk or this wild D&D extension you buy last month ... and make money in return. 
_____________________________________________________________

## **The Stack**

Javascript, HTML, CSS

Front:
+ React,
+ Redux, 
+ Sass,
+ Axios

Back:
+ NodeJS,
+ Sqitch,
+ PostgreSQL,
+ Express (Active Record)

_____________________________________________________________

### To run Oboardgame locally :

Please be sure to have installed PostgreSQL and Sqitch properly and have every authorizations needed to create a database & interact with it.

* Clone repo on `main` branch
* Create a new database locally with `create database oboardgame`
* In terminal, get in _FRONT_ folder with `cd FRONT/`  & do `npm i` to download dependecies
* Now for the _BACK_ folder : `cd ../BACK/` then `npm i`
* After this you will need to deploy the migrations with `sqitch deploy db:pg:oboardgame`
* Then insert datas from the localisation API file in there with `node app/services/localisationAPI.js` (this is for the french cities names & zipcodes from french government's API)
* Wait a few seconds, (there is many cities in France ...)
* Then the fakes datas for some users and ads with `psql -d oboardgame -f data/import_data.sql`

If everything is right , you should now be able to launch the application.

To do so : 

* `node index.js` in the _BACK_ folder to launch local server
* `yarn start` in the _FRONT_ folder to launch front in your browser

Here is the V1 of Oboardgame.

Everyone in the team involved his best in this realisation, in one month deadline, after five month of intensive learning in a new professional branch for each of us.

We do want to continue the development of Oboardgame, stay tuned for potential evolutions.

Hope you like the concept !

__Cédric Leizour__ - *Scrum Master & Frontend Developper on Oboardgame*
