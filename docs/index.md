# Welcome to Carpool and Go!

## Table of contents
* [Group Member Agreement](#group-member-agreement)
* [Overview](#overview)
* [Project Goals](#project-goals)
* [Touring the Interface](#touring-the-interface)
* [What the system Should Eventually Provide](#what-the-system-should-eventually-provide)
* [Development Mockup Pages](#development-mockup-pages)
* [Development History](#development-history)
* [Deployment](#deployment)

## Group Member Agreement
This web application is made in cooperation with [Kenji Sanehira](https://sanehirakenji.github.io/), [Cory Parker](https://hnlcory.github.io/), [Robin Dumlao](https://robindum.github.io/ ), [Michael Ito](https://michaelbito.github.io/), [Johanan Leoncio](https://johanancs.github.io/ ), and [Kai Sequeira](https://kaialii.github.io/).

For more information on the creation and the distribution of work, to contribute as a team, you can check [here.](https://docs.google.com/document/d/1YAd3LihnKsh5QRUVU11w1N1Rn5ffM7UGuOMRcv6_smM/edit?usp=sharing)

## Overview
Carpool and Go! is a web application project mockup that aims to provide a communal network for University of Hawaii at Manoa, allowing for drivers to offer rides and for riders to be able to search for rides in their area. Click [here](https://github.com/carpool-and-go) to see the github organization for this project.

## Project Goals
Our goal with this project is to take in what we have learned over the course of the semester to create a functioning meteor application that reflects the teachings as well as the creative freedoms we get to choose while creating this project. By working together in a team environment, we aim to gain experience as well as further our practice in web design. Also, by creating a mockup for a service in an attempt to combat a real world problem, we hope to be able to translate this problem solving into other scenarios in real world applications.

## Touring the Interface
As we progress and further develop the website application, we will be showing the different aspects of our website and pages here. This is where the final product and how to navigate through the website will go. Currently there is nothing yet, but stay tuned!

    Pages (WIP) //this will be describing what users see when they first enter the
    website, how to create an account, what can they do after, etc.

## What the System Should Eventually Provide
What this system should eventually provide is a website service that allows University of Hawaii at Manoa students and staff the ability to have access to get to school with having less cars needed to traverse the roads. Users who log in can either look to offer rides, or search for possible drivers that they can catch a ride with to campus. By offering this service, we hope to do our part to help against the rising gas prices and heavy traffic near the University.

## User Guide
This section serves to guide the user through the currently implemented features of Carpool and Go. After reading through it, the user should have a general idea of how the site works and how to use it to the best of their ability.

### Landing Page
The landing page will contain a general description of what Carpool and Go aims to accomplish:

![](https://media.discordapp.net/attachments/251791549866835968/961702566247424020/LandingPage.PNG?width=910&height=453)

### General Home Page
The general home page will look similar to digits, in that it contains three columns that describe the specific functions of the site:
* Drivers
* Riders
* FastRide

![](https://user-images.githubusercontent.com/97719124/163473129-15cf6039-5b62-4e31-adb3-be3354dcbba3.png)
![](https://user-images.githubusercontent.com/97719124/163473220-0e9e8f30-da0a-42ee-a853-38ec2b91b27a.png)

### User Profile Page
The user profile page will be a large card that contains all of the fields required of the user when they log in. At the bottom of this card will be an edit section, which the user can click on that will take them to the "User Profile Edit Form".

![](https://user-images.githubusercontent.com/54416383/163450377-c63fbeb6-682d-4819-8ef5-32c887b6073c.png)

### User Profile Edit Form
The user profile edit form will be a form that contains all of the fields required of the user when they log in. It will change only the data of the current user logged in, and upon submitting, will change the users data in the user collection and the users data in the User Profile Page.

![](https://user-images.githubusercontent.com/98077871/163379749-84f6d5aa-b80c-4c54-8258-80ae5fcec245.png)

### Drivers/Riders Page
The Drivers/Riders Pages will be nearly identical in structure, but will differ in the data they display. The Drivers page will show exclusively drivers whereas the riders will only show riders. The top of the page will contain a filter container that allows the user to sort by location.

![](https://user-images.githubusercontent.com/97719124/163475875-6688ac19-6721-47c5-b803-43dbb8268751.png)

### "Fast Ride" Feed
The "Fast Ride" feed page will be a feed that consists of all of the requested Fast rides sent by the Fast Ride Form. The feed will display the user's Profile Picture, their first and last name, and then the rest of the information gathered from the fast rides form.
This is similar to the digits notes feed shown below:

![](https://cdn.discordapp.com/attachments/251791549866835968/961703096411631616/FastRideForm.PNG)

### "Fast Ride" Form
The "Fast Ride" form page will be a form that allows a user to request a ride to a specific location at a particular time of day. It will send data to the "Fast Ride" feed.
This is similar to the digits notes form shown below:

![](https://user-images.githubusercontent.com/31085175/163355483-6dc26354-d852-4809-94ad-cb8f06085dee.png)

## Developer Guide
--Insert stuff here--

## Development History
Milestones are important! This project undergoes the developmental process practices in order to create a fully functioning meteor proof-of-concept prototype. This section is dedicated to keeping track of milestone goals and how we managed to achieve them.

### M1 Milestone
Our M1 Milestone was essentially developing the basic skeleton of the website, implementing collections we will be using in the project, and correcting the routing of the bowfolios template to match our website. We had a total of 13 issues for this Milestone, and the project board can be found [here.](https://github.com/carpool-and-go/carpool-and-go/projects/1) 

![](https://cdn.discordapp.com/attachments/930054006812844065/964423632124256266/Final.JPG)

### Finished Issues:
* Implement the Profiles Collection
* Implement the Locations Collection
* Create General Presentation
* Edit Navbar and Footer
* Clean up Sign in, Sign Up, and Landing Page
* Implement Riders List Page
* Implement Drivers List Page
* Implement the User Profile
* General Home Page
* App.jsx Routing
* Implement Edit Profile Page
* Successful Sign-in Redirect
* Implement Fast Ride Form Page
* Deploy Carpool and Go to Digital Ocean
* Set up domain name and https for our final project

### M2 Milestone
Now that the mockup of the pages and the skeleton of the website is complete, it is now time to focus on functionality and making things work together. The goal of this milestone is to have a working site with no broken links. Check out our [M2 project board.](https://github.com/carpool-and-go/carpool-and-go/projects/3)

Finished Project Board:
-- INSERT FINISHED M2 IMAGE HERE --

### Finished Issues:
* Fixed Image Proportions
* Implement General profile page viewer for cards
* Implemented create profile page
* Figure out how to update location role in edit profile
* Finish the edit profile page
* Update homepage screenshots
* Hide sign in / sign up buttons when logged in
* Implement default login users with one user being an admin
* Change driver/rider collection to show current user
* Implement admin page
* NavBar - remove edit profile from the navbar, change Icon
* SignUP fix Profiles.Insert
* Add 15 default driver data
* Add 15 default rider data
* Implement basic tests for website
* Start looking into a possible Rating System
* Finish Fast Ride Feed/Form

### M3 Milestone
Now that we have the general features of the website completed. Finish off the site by fixing minor UI bugs, implementing the sites "secret sauce", and essentially complete the project as a whole. Check out our current [M3 project board.](https://github.com/carpool-and-go/carpool-and-go/projects/4)

Current Project board:
-- INSERT HERE --

## Deployment
The following is a link to our deployed application running on Digital Ocean:
Click [here.](http://167.71.66.48/)
