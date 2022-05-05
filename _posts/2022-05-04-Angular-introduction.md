---
layout: post
title:  "Angular introduction"
date:   2022-05-04 18:05:50 -0700
categories: General Posts
author: Wyatt 
---

This post showcases a small app built using Angular: a front end framework like React or Vue, but one that is much larger and more involved than any other front end framework.  

There is definitely a bigger learning curve to Angular and building a small app doesn't make me proficient; however going through step by step this simple task tracker application here is what I have learned -
- I understand how components are created, why they are used and how they communicate across the functionality of the parent components. For example the add task button catches a users click of the add button, fires off an Event Emitter in the corresponding typescript file and then delegates the handling of the event to the parent task component.
- Angular Services support components by interacting with the mock database used for the project: db.json. The tasks service uses http requests to get the current tasks, delete a certain task, add a task or toggle a reminder(CRUD); the functionality and logic to update the UI is passed back to the corresponding components typescript file. For example after deleting a task entry in the server the task item component will filter the tasks array using .filter(). Additionally there is a UI services file that supports toggling the view of the tasks upon pressing the ‘add’ button as well . From here, using *ngIf on the entire form in the add-task html toggles the add task form to appear and disappear.
- Observables are used for asynchronous programming in Angular such as communicating with the backend for CRUD operations. Observables can be accessed in the component .ts files through the .subscribe() method and can call a function in one of the services, manipulate the server and pass back data to be updated in the UI.
- An understanding of the module system, along with imports and exports are important to using all the required packages and dependencies of your Angular project

There is more I could say about all the properties and methods I learned, however I wanted to cover what I thought are the main ideas. In the future I'd like to rewrite the front-end of my crypto-currency notification website using Angular (and add some stuff along the way) .. look out for an update one day


You can visit the source code [here](https://github.com/wyattcolyn/AngularIntroduction/tree/main){:target="blank"}