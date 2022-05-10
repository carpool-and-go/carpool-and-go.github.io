# Welcome to Carpool and Go!

## Table of contents
* [Group Member Agreement](#group-member-agreement)
* [Overview](#overview)
* [Project Goals](#project-goals)
* [What the system Should Eventually Provide](#what-the-system-should-eventually-provide)
* [User Guide](#user-guide)
* [Developer Guide](#developer-guide)
* [Development History](#development-history)
* [Community Feedback](#community-feedback)
* [Deployment](#deployment)

## Group Member Agreement
This web application is made in cooperation with [Kenji Sanehira](https://sanehirakenji.github.io/), [Cory Parker](https://hnlcory.github.io/), [Robin Dumlao](https://robindum.github.io/ ), [Michael Ito](https://michaelbito.github.io/), [Johanan Leoncio](https://johanancs.github.io/ ), and [Kai Sequeira](https://kaialii.github.io/).

For more information on the creation and the distribution of work, to contribute as a team, you can check [here.](https://docs.google.com/document/d/1YAd3LihnKsh5QRUVU11w1N1Rn5ffM7UGuOMRcv6_smM/edit?usp=sharing)

## Overview
Carpool and Go! is a web application project mockup that aims to provide a communal network for University of Hawaii at Manoa, allowing for drivers to offer rides and for riders to be able to search for rides in their area. Click [here](https://github.com/carpool-and-go) to see the github organization for this project.

## Project Goals
Our goal with this project is to take in what we have learned over the course of the semester to create a functioning meteor application that reflects the teachings as well as the creative freedoms we get to choose while creating this project. By working together in a team environment, we aim to gain experience as well as further our practice in web design. Also, by creating a mockup for a service in an attempt to combat a real world problem, we hope to be able to translate this problem solving into other scenarios in real world applications.

## What the System Should Eventually Provide
What this system should eventually provide is a website service that allows University of Hawaii at Manoa students and staff the ability to have access to get to school with having less cars needed to traverse the roads. Users who log in can either look to offer rides, or search for possible drivers that they can catch a ride with to campus. By offering this service, we hope to do our part to help against the rising gas prices and heavy traffic near the University.

## User Guide
This section serves to guide the user through the currently implemented features of Carpool and Go. After reading through it, the user should have a general idea of how the site works and how to use it to the best of their ability.

### Landing Page
The landing page will contain a general description of what Carpool and Go aims to accomplish:

![](https://media.discordapp.net/attachments/251791549866835968/961702566247424020/LandingPage.PNG?width=910&height=453)

### General Home Page
The general home page after logging in will present the user with a number of options including viewing drivers/riders, editing their profile, and accessing the fast ride feed.
![](https://cdn.discordapp.com/attachments/959715872673521695/968625542096117770/Home1.PNG)
![](https://cdn.discordapp.com/attachments/959715872673521695/968625542494564352/Home2.PNG)

### User Profile Page
The user profile page displays the User in question's profile as well as their role, location, profile picture, arrive and leave time, contact information, and their rating. The user profile page will also show the user's current rating and how many people rated them. There is also a section where other users can submit ratings for the current user (if the user is not the one logged in). If the profile is the current logged in user's profile, there will instead be an "edit my profile" link that takes them to their respective edit my profile. Users can also delete their own profile if they would like to.

![](https://cdn.discordapp.com/attachments/474906296819253268/973493095658319892/unknown.png)

If the user does not have a profile, they will be prompted to make one using the add profile page (See below).

![](https://cdn.discordapp.com/attachments/959715872673521695/968625569073873007/UserProf2.PNG)

### Add/Edit profile page
The Add/Edit profile page will be a form that contains all of the fields required of the user when they log in. It will change only the data of the current user logged in, and upon submitting, will change the users data in the user collection and the users data in the User Profile Page.

![](https://cdn.discordapp.com/attachments/474906296819253268/973492312011341824/unknown.png)

If the user does not have a profile, they will have to create their profile.

![](https://media.discordapp.net/attachments/959715872673521695/968625569442975744/AddProf.PNG?width=819&height=670)

If the user is not an admin or not a user in question, they will get a message saying "you do not have access to this profile".

![](https://media.discordapp.net/attachments/959715872673521695/968625603425210408/No_Access.PNG?width=881&height=329)

### Drivers/Riders Page
The Drivers page will show exclusively drivers whereas the riders will only show riders. The top of the page will contain a filter container that allows the user to sort by location. These collections of drivers and riders will also display if the rider or driver is a highly rated profile or a lower rated profile based on the rating property.
#### Drivers Page
![](https://cdn.discordapp.com/attachments/474906296819253268/973491719003865098/unknown.png)
#### Riders Page
![](https://cdn.discordapp.com/attachments/474906296819253268/973492118326771752/unknown.png)

### "Fast Ride" Feed
The "Fast Ride" feed page will be a feed that consists of all of the requested Fast rides sent by the Fast Ride Form. The feed will display the user's Profile Picture, their first and last name, their current and desired locations, the time they need a ride, a brief description of their requested ride, and their contact information. Other users can then contact the user or click on their profile to get more information about that specific user.

![](https://cdn.discordapp.com/attachments/474906296819253268/973491502095421460/unknown.png)

### "Fast Ride" Request
The "Fast Ride" request page is a form that allows a user to request a ride to a specific location at a particular time of day. It allows the user to input their current and desired locations, their time of ride, and a description of why they need the ride. It will send data to the "Fast Ride" feed.

![](https://cdn.discordapp.com/attachments/474906296819253268/973491306733129748/unknown.png)

### Rating System
The rating system is an implementation that allows drivers and riders to be able to rate their fellow community members based on experiences. These ratings seek to create a positive incentive to those who ride with Aloha! Users are able to rate drivers and riders out of 5 stars. The rating can be seen on one's profile, and to rate others would show up on other profiles as shown:

#### Self Rating:
![](https://cdn.discordapp.com/attachments/959715872673521695/973388057086664754/selfRating.png)
#### Rating Others:
![](https://cdn.discordapp.com/attachments/959715872673521695/973388066569998336/rateOthers.png)

### Admin Page
The admin page is a page that is similar to the drivers/riders page in that it displays the profiles based on their locations (filtered by a small filter container), however each profile also has an edit profile button that allows an admin to edit their profile. Admins can also delete profiles if they need to with the delete profile button.
![](https://cdn.discordapp.com/attachments/251791549866835968/973504507604520990/NewAdmin.JPG)

### Night Light Mode
Carpool and Go has implemented a darker theme colors for those night time browsing! By clicking on the circular button at the bottom right of the screen, the colors invert to make things more pleasing to the eyes:
![](https://media.discordapp.net/attachments/474906296819253268/973483093145059388/unknown.png?width=1076&height=571)

## Developer Guide

This section provides information of interest to Meteor developers wishing to use this code base as a basis for their own development tasks.

### Installation

First, [install Meteor](https://www.meteor.com/install).

Second, visit the [Carpool and Go application github page](https://github.com/carpool-and-go/carpool-and-go), and click the "Use this template" button to create your own repository initialized with a copy of this application. Alternatively, you can download the sources as a zip file or make a fork of the repo.  However you do it, download a copy of the repo to your local computer.

Third, cd into the bowfolios/app directory and install libraries with:

```
$ meteor npm install
```

Fourth, run the system with:

```
$ meteor npm run start
```

If all goes well, the application will appear at [http://localhost:3000](http://localhost:3000).

### Application Design

Carpool and Go is loosely based upon [Bowfolios](https://github.com/bowfolios) and [meteor-example-form-react](https://ics-software-engineering.github.io/meteor-example-form-react/). Please use the videos and documentation at those sites to better acquaint yourself with the basic application design and form processing in Bowfolios.

### Data model

As noted above, the Bowfolios data model consists of three "primary" collections (Projects, Profiles, and Interests), as well as three "join" Collections (ProfilesProjects, ProfilesInterests, and ProjectsInterests).  To understand this design choice, consider the situation where you want to specify the projects associated with a Profile.

The Carpool and Go UH collection consists of three primary collections (Users, Locations, and Notes). There is also a "join" collection "UsersLocations" that allows the database to access a User's role and location both ways. The notes collection is currently a placeholder for the different entries into the FastRideFeed.

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
* Fixed showing user location in edit page

### M2 Milestone
Now that the mockup of the pages and the skeleton of the website is complete, it is now time to focus on functionality and making things work together. The goal of this milestone is to have a working site with no broken links. Check out our [M2 project board.](https://github.com/carpool-and-go/carpool-and-go/projects/3)

Finished Project Board:
![](https://cdn.discordapp.com/attachments/959715872673521695/968619832088092682/M2_board.png)

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
After implementing the general features of the website, we finished off the site by fixing minor UI bugs and implementing the sites "secret sauce". Check out our [M3 project board.](https://github.com/carpool-and-go/carpool-and-go/projects/5)

Finished Project board:
![](https://cdn.discordapp.com/attachments/697982688484786187/973377437557723176/M3.JPG)

### Finished Issues:
* Implement Dark Mode
* Implement Google Maps in Landing Page
* Insert the property "rating" as "0" when a user adds their profile
* Fix padding in UI
* Fix Fast Ride Feed
* Fix Edit Page button on HomeDR
* Have loaction preset when editing a profile.
* Update photos on homepage to reflect final ui
* Userview shows "edit page" button when the current user is logged in
* Allow deletion of profiles from the admin page
* Fix the homeDR page having a smaller navbar
* Add real appropriate images (or data) for the final project
* Add placeholders fro the current forms in order to allow the user to see how the form is supposed to look
* Fix the delete function such that the user is not fully deleted and instead the user's data is reset
* Add delete profile to the User's profile
* Create admins when accounts signup with specific email "@carpoolngo.com"
* Finalize Tests for the final Milestone
* Cleanup/Optimize Code
* Fully Implement Rating System
* Fix bug that when the user is created they recieve an immediate low star rating
* Get admin page to refresh cards when a deletion occurs.
* Update Homepage with final UI screenshots.
* Collect Community Feedback, 1 Student Each.
* Bug: Logged in as admin, no account, went to admin page, edit another users account, said “add user” instead of “edit”, submission creates another account of that person, deletion destroys admin page

## Community Feedback
While testing the website in its final stages, we took the time to get some thoughts and opinions from other UH community members. Since this aims to serve as a service for those who attend UH Manoa, faculty and fellow UH at Manoa students were asked on what they thought.

`"I really liked the visuals, and the page is very user friendly. The site seems very modern and not outdated. I would enjoy using an app like this. "`

`"I actually really like this idea and design; I hate spending a lot of money on gas driving to school. I was pretty surprised at how well the website worked and turned out, I thought it would be something simpler since you said it was just an assignment or something. I could make an account and sign in and everything so that was pretty cool. I could even sort profiles by certain categories. Some of the interfaces were slightly clunky, but nothing that was a big problem for me."`

`"The site looks great besides the unfinished portions. One comment would be the full implementation of the dark mode of the website and working with different fonts and stuff."`

`"I find it a bit hard to imagine there will be willing drivers since there is an app like uber which is a similar concept but drivers are incentivized. It's easy to see riders willing to do this, but if people do not know who they are picking up it is difficult to see who would be willing to do this. Maybe add a feature where riders have a rate or small fee of pickup and dropoff. It would be good to add a map on google rather than a dropdown menu for the rider and driver pages. You could add a background check option for drivers and riders for security purposes."`

`“So there’s this little location tab Arrive time and leave time. I feel like if you could make the tabs more user friendly that would be easy for the users. Also on the arrive time and leave time some websites have it where the user can just click on the time instead of typing it out. So if you can give an option of clicking instead of typing would be more user friendly. `

To summarize, these different bits of feedback mainly commented on things that we are able to develop further if we were to revisit this project. These include an incentive system for drivers, varying form fields, user interface changes, and all in all making the website more user friendly.

We have taken this feedback into consideration and appreciate the community for giving us such gracious criticisms and praise. We aim to create a service that benefits all those involved and with more time we can continue to create something that everyone can gain from.

## Deployment
![ci-badge](https://github.com/carpool-and-go/carpool-and-go/actions/workflows/ci.yml/badge.svg)

The following is a link to our deployed application running on Digital Ocean:
Click [here.](https://uh-carpool-and-go.xyz/#/)
