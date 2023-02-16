# AlumniWebsite

<!--Content Table-->

## Content 

- [Effat University Book Club](#effat-university-book-club)
  * [Purpose](#purpose)
  * [Description](#description)
  * [FRONT-END](#front-end)
    + [Website Layout](#website-layout)
      - [Home](#home)
        * [Join Us](#join-us)
        * [Log In](#log-in)
          + [Profile](#profile)
          + [Book Read](#book-read)
      - [About Us](#about-us)
      - [Event](#event)
        * [Manage Event](#manage-event)
      - [Club Members](#club-members)
      - [Book List](#book-list)
        * [Edit Book](#edit-book)
        * [Delete Book](#delete-book)
  * [Back-END](#back-end)
    + [Members](#members)
    + [Books](#books)
    + [Events](#events)
    + [Event Attendance](#event-attendance)
    + [Messages](#messages)
  * [Files](#files)
    + [CSS](#css)
    + [Javascript](#javascript)
  * [Enhancement](#enhancement)
  * [Getting Started](#getting-started)
    + [Dependencies](#dependencies)
    + [Installing](#installing)
    + [Viewing the Website](#viewing-the-website)
      - [How to view the website](#how-to-view-the-website)
      - [How to view the database](#how-to-view-the-database)
    + [Help](#help)
  * [Authors](#authors)
  * [Acknowledgments](#acknowledgments)


## Purpose
<!--Purpose of the project-->
This poject is a website dedicated for Effat University book Club (leader and members). 

<img src="https://github.com/AichaSidiya/AlumniWebsite/blob/main/demoAlumni.gif"/>

<!--Header 2 description of the project-->
## Description

<p style="text-align: justify;"> This project will create a database for the club where the name, email and id of the members will be stored, it will also store a list of all the books they read and the events they organized. The website will display this information for all users, but it will also include a join us option for any new student who would like to be part of the club. After registering a student will log in and a profile will be created for her. The profile can be edited or deleted by the student. She will also be able to fill a form to discuss the book she read; she can later edit it the form. All users can register to attend the events organized by the club. Finally, the admin which is the club leader can add new event or edit existing ones and can delete books from the database.A contact option is also provided any user can leave a message to the club.</p>

<!--Header 3 front end-->
## FRONT-END
We have a total of 19 pages.

### Website Layout

#### Home
* Main activities that the club provide. 
* Joining or logging in.
* Contact the club. 

##### Join Us 
* Clicking on the join us button will lead the user to a form where she will fill her personal information including her name, id, email password...

##### Log In
* Clicking on the log in button will lead the user to a form where she will fill her id and password and the website will check if it matches tha data in the databse then it will welcome the user.

###### Profile
* Upon logging in the log in and join us buttoon will disapear, a logout option will appear on the menu and a profile page will be created with a edit and delete option.
* The edit option will display a form of the user info.
* Note that the admin can't delete her account she can only update the name and id and pass.

###### Book Read
* Club Members also have the option to add books by filing the form in the book read page that will appear in the menu upon logging in.

#### About Us
* In the upper menu a user that is not a member can browse to the about us page where a "Be Part of Our Family" will take her to the join us form. 

#### Event
* In the upper menu a user that is not a member can browse to the event page 
* View and register to attend an events.
* Manage event button for the admin.

##### Manage Event
* Clicking on the mange event button will take the admin to a page were she can add or edit or delete event. 
* The add and edit event will take her to a form page to fill the required information.

#### Club Members
* In the upper menu a user that is not a member can browse to the club members page that lists all the club members, and provides genral info about them such as the genre they like and a small welcome message. It also indicates the leader of the club. A menu is provided to be able to go read about a particular member.

#### Book List
* In the upper menu a user that is not a member can browse to the book list page that lists all the books that the club read till now, and provides genral info about it such as the title, author and genre of the book in addition to a small summary.
* Edit Book button for members and admin.
* Delete button for the admin.

##### Edit Book
* Clicking on the edit book button will take the member to a page were she can edit the chosen book. 
* The member has to fill the required information of the book.

##### Delete Book
* Clicking on the delete book button will take the member to a page were she can delete the chosen book. 
 

## Back-END

We have 5 tables in our database

### Members
* Includes all the member information extracted from the join us form.
### Books
* Includes all the book information exctracted from the book read form.
### Events
* Includes all the event information exctracted from the add event form.
### Event Attendance
* Includes all the student and event id.
### Messages
* Includes the message and the the contact information of the user who left the message.


## Files
### CSS

* Ourstyle.css
* booklist.css
* clubMembers.css
* styles.css


### Javascript

* Bookread.js
* Deletebook.js
* Editbook.js
* Editevent.js
* Editprofile.js
* eventRegistration.js
* myScript.js
* newevent.js
* scripts.js

## Enhancement
* Send the contact us message to the vlub email.
* Make non members caable of registering to attend the club event by changing the format of the register now form.
* Add a back up button to the club members and book list pages
* Add a menu and a back up buttoon to the event page for the each event
* Add a more button to the each book in the book list and hide some the summary
* Create an discssion board for each book and each event were more information is displayed and a discussion is provided via comments, in addition to a rating option.
* Show the ration of the event and the book in the event and booklist page.


<!--Header 3 installation and launching the project-->
## Getting Started

### Dependencies

<!--Link to install the latest version of g++-->
* This project is hosted on xampp and phpmyadmin. You will need to download xxamp to see it. a link is provided.
* [xampp](https://www.apachefriends.org/download.html)

### Installing
<!--Steps of Installation-->
* Download the xampp and install it. 
* Download the zip file and create a folder for it.

### Viewing the Website
<!--Steps for running the program-->
#### How to view the website
* Look for Xampp Control Panel in your search bar

![1](https://user-images.githubusercontent.com/91727165/147794092-3998f103-99bd-4560-835b-bfe9f7154c9c.png)

* Start Apache and MySQL

<img width="500" alt="2" src="https://user-images.githubusercontent.com/91727165/147794319-03138add-f182-4889-8fde-ab9adc36610a.PNG">

* Search in your browser for:
```
localhost/index.php 
``` 
and then start browsing the website

#### How to view the database
* Search for:
```
localhost/dashboard/
``` 

* Then search for phpMyAdmin

![3](https://user-images.githubusercontent.com/91727165/147794096-fd8bc2ed-3721-4794-abfc-d10dfbce0831.png)

* To check the database create a new database in phpmyadmin named bookckub then upload the given sql to the newly created database, by clicjing on import and import the provided bookclub sql.


![7](https://user-images.githubusercontent.com/91727165/147794091-56156a25-6edb-4ac6-a7af-7deeb11d7d50.png)

![6](https://user-images.githubusercontent.com/91727165/147794090-8681a72f-3058-4903-9090-1cd248538fb3.png)

![5](https://user-images.githubusercontent.com/91727165/147794089-0afc66d5-b13d-49d6-84bd-853f4bbe08f6.png)

![4](https://user-images.githubusercontent.com/91727165/147794088-72eb10ec-1dcf-4419-8c98-e1243be89924.png)


### Help
If the changes in the website does not appear try using another browser or click on Fn + F5

## Authors
<!-- The contributors to the project-->
* [Aicha Sidiya](https://github.com/AichaSidiya)
* [Hanin AlZaher](https://github.com/hanin-az)
* Razan AlMahdi
* Layal Ghiryani


## Acknowledgments
<!-- Insparation files, codes, and general refrences used in writing the code of the project-->
* [BootStrap used](https://startbootstrap.com/previews/agency)
* [CSS grid style](https://stackoverflow.com/questions/47587892/how-does-css-grid-layout-works)
* [Readme Template](https://gist.github.com/DomPizzie/7a5ff55ffa9081f2de27c315f5018afc)
* [Readme Content Table](https://ecotrust-canada.github.io/markdown-toc/)
