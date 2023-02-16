

# ShakeIt: Cocktail recipes Mobile App
<b> Contributors: [Oliwia](https://github.com/Olive-kaa), [Ben](https://github.com/bsmith), 
[Gintare](https://github.com/GINTARE07) & [Mikhail](https://github.com/MikhailGorbunov) </b>



A full stack React Native mobile application (Android) that allows users to install it on an Android phone, be able to search for a cocktail recipe, leave a comment, and (as an extension) personalise the experience . We will use Firebase database to store the recipe and user data.

<!-- restaurant bookings through their unique profile. They can browse restaurant availability, create/review/delete bookings, as well as adding restaurants to their favourites. The backend is built in Java with Spring. -->

<!-- 🚧 <b> NB: This is app has reached its MVP, but is still under construction</b> 🚧 -->


## Contents 

* [Idea](#idea)
* [Showcase](#showcase)
* [Technologies](#technologies)
* [Brief](#brief)
* [Challenges](#challenges)
* [Running a ShakeIt demonstration](#Running a ShakeIt demonstration)
* [Example Data](#Example Data)
* [Test](#Test)

<br>

## Idea

Every day the human body needs food and water. Therefore, people either cook or order food online. To cook, you need to find food recipes make a shopping list, and tick each item in the list while shopping. You can use pen and paper but it's not environmentally friendly. You can type in your phone's notes but it takes some effort. That's the time when users load an app. And for food recipes, there are plenty of apps. But what about cocktails?

<br>

## Showcase

https://user-images.githubusercontent.com/68015812/219238487-7fe6d5c0-e4b5-430f-aaf6-7c4bf5910944.mp4

Full app expirience is avaialable at 
https://www.youtube.com/watch?v=WsNRsFLqt1Y&t=1s


<br>


## Technologies

These are the main technologies we used to contruct the project.

* ![stats]
* ![ReactNative]
* ![Java]
* ![JavaScript]
* ![Tailwind]
* ![Firebase]


<br>


## Brief
Our initial brief was extremely ambitious, so as our team. Together through learning from scratch react native liblary and firebase database we have managed in two weeks time to accomplish the following tasks (shown bellow).

**MVP**


- [x] Display recipes (with images)
- [x] Be able to search cocktail recipe by name
- [x] Data is stored in a database accessible through a RESTful API
- [x] Have a README file with screenshots/videos and running instructions.

<!-- API find or make -->

**Extensions **

Some of the features currently in progress:

- [x] Be able to leave a comment under each recipe
- [x] Have a two colour scheme being both accessible (dark and light)
- [x] Comments have tags 
- [x] Recipe can be searched by the tag
- [x] Be able to search cocktail recipe by ingredient
- [x] Calculate recipe portion 
- [x] Be able to login 
- [x] Be able to add recipe to a shopping list
- [ ] Be able to customize recipe

**Super Extensions **

- [x] Add a cloud (Firebase)
- [ ] Create a shopping bot 
- [ ] Be able to add recipe to a party planner 
- [ ] Create an email invitation
- [ ] Be able to make their own recipe 
- [ ] To be able to upload the app to google play

<br>

## Challenges

Here are some of the things we've found difficult:

* Learning a new framework while planning & building 
* Learning how Reactive Native works
* Making our database connect with our mobile app
* File structuring & naming conventions as the project scaled up in size
* Managing dependency and version issues


<br>



## Running a ShakeIt demonstration

A ShakeIt demonstration consists of three parts:

* an Android app built with React Native and Expo Go
* a database and authentication service provided by Firebase
* a search service provided by a Java Spring Boot application

### Running the Java Search Service

ShakeIt uses a Java+Spring+Firebase server to provide a HTTP/REST API for searching
for recipes.

Before running the server you need to configure a `serviceaccount.json` file in the `ShakeItSearch` directory.
Go to the [Firebase Admin Console](https://console.firebase.google.com/) for your project.  Select \[cogwheel\] -> 'Project Settings' -> 'Service Accounts'.
Select 'Java' and the 'Generate New Private Key' button.

To build and run ShakeItSearch, just use this command in a new terminal.  You will need to keep this running while using the app.

```
(cd ShakeItSearch && ./build_and_run)
```

Alternatively, open ShakeItSearch in IntelliJ where you can run the `ShakeItSearchApplication` or the tests.

Finally, to allow the Android app to contact the search service we are going to use
[ngrok](https://ngrok.com/).  In another terminal you need to use the following command.  It writes
a `searchConfig.js` file for the Android app after starting an ngrok tunnel.

```
npm run ngrokSearch
```

## Example data

Example data for loading into a Firebase realtime database is in the files `data/examples/*.json`.

The JSON files are generated by data in the JS files in the `data/examples/` directory. To regenerate the JSON files, run `npm start` in the data/ directory.

## Tests

The application logic in ShakeIt in tested with [mocha](https://mochajs.org/).

Run the tests with `npm test` in the ShakeIt directory.




<!-- MARKDOWN LINKS & IMAGES -->

<!-- [ReactNative]:https://img.shields.io/badge/React_Native-20232A?style=for-the-badge&logo=react&logoColor=61DAFB -->
[Java]:https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white
[Spring]:https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white
[Hibernate]:https://img.shields.io/badge/Hibernate-59666C?style=for-the-badge&logo=Hibernate&logoColor=white
[PostgreSQL]:https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white
[IntelliJ_IDEA]: https://img.shields.io/badge/IntelliJ_IDEA-000000.svg?style=for-the-badge&logo=intellij-idea&logoColor=white
[ReactNative]:https://img.shields.io/badge/React_Native-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[stats]:https://img.shields.io/tokei/lines/github/bsmith/ShakeIt
[Tailwind]:https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white
[Firebase]:https://www.vectorlogo.zone/logos/firebase/firebase-ar21.svg
[JavaScript]:https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black

