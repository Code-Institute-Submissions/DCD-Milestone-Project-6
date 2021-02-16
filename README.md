# The Game Corner
The Game Corner is a website dedicated to compiling and providing reviews of video games. 
The website allows user input to search for and view information about various video games, as well as allowing them to write their own reviews, to recommend or criticise the respective video game.
Additionally, new games can be added and removed by the admin.

## User Experience (UX)
The goal of this website is to provide a satisfactory user experience and allow video game fans and critics to write their own opinion pieces on popular video game titles.
The website should allow users to easily log in or register, and search for the video game title they wish to view.
The user should then be able to easily add or edit their reviews as well as view reviews ceated by other users.

### User Stories
1. As a user, I would like to be able to search for specific video games and look at reviews.
2. As a user, I want to create an account so I can add my own reviews.
3. As a user, I want to log in to my existing account to add or edit my reviews.
4. As a user, I want to be able to save my review for other users to view.
5. As an admin, I want to add new games to the site for users.

### UX Framework

**1. Strategy**

The Game Corner is a video game review website with front-end and back-end functionality, created using HTML, JavaScript, CSS, Python, Flask, and MongoDB.
The goal is to create a website that is user-friendly and allows users to easily find and review video games.

**2. Scope**

The website should be interactive and allow users to unput their own reviews for other users to see, as well as allowing them to edit their content, and search for different games.
They should also be able to provide a rating for the game as part of the review.

**Functional Requirements**

Functional requirements include: a user-friendly navigation menu, a search bar, working templates for games and reviews to be added, database functionality that stores user login information and ability to create new accounts, with authentication.
In addition, the website should be responsive for various screen sizes, whilst maintaining the same level of functionality.
The main functionality of the website is to allow users to create, read, update, and delete data, known as CRUD. 
The data created is stored in a database, and can be read through various pages on the website. The users also have the option to update and edit the data they have submitted, as well as delete it altogether.
A search field allows users to search for specific titles they are interested in

**Content Requirements**

The content of the site should include a header and image, as well as a navigation menu. 
A search bar should allow users to search for video game titles.
For each game, an image should be included, as well as its title, the genre of the game, and a short description of the game.
An input field for users will allow them to add reviews for each game, and they are also able to provide a rating, which will be compiled as a list alongside other user reviews.

**3. Structure**

The website is structured to allow new vistors to view the games and reviews on the landing page once they open the website. 
From there, they are able to log in or register, which will allow them to view their profile page of existing reviews.
Once logged in, users are able to click on the 'View Games' link, which allows them to search for games, and add or edit reviews. They are able to then save the review.
Once the user wishes to end their session, they can click the 'Log Out' option in the menu to return to the home page.

**4. Skeleton**

The skeleton of the website will utilise Materialize for the CSS layout of the pages. A navigation menu will allow users to go to their chosen pages.
The 'View Games' page aims to integrate the home page layout with the option for users to add their own data. This minimises the need for different pages for users to visit and provides a seamless experience.
When adding or editing a review, a drop down text input box will open for users to add their text and rating, and save it.
Additional optiions in the navigation menu allow the user to navigate back to their own profile, or to end the session and log out.
This simplifies the number of options for the user and keeps the website easy to use.

**5. Surface**

The surface design of the website will also utilise Materialize CSS to provide a theme and styling for the components of the website.
Google Fonts is used to style the text, and FontAwesome is used for various icons.
The colour scheme is designed to be visually appealing to the target audience of gamers, and provide clear readability as well as being responsive.

### Wireframe

My wireframe was created using the Balsamiq program, and shows the basic layout for the website in desktop as well as responsive formats such as smartphones and tablets.
Notes describing each wireframe are included below each page of the PDF, linked below.
[Wireframe PDF made in Balsamiq](/workspace/DCD-Milestone-Project-3/MS3-wireframe.pdf)

## Features

### Existing Features

1. Register functionality
2. Login functionality
3. Log out functionality
4. Profile page
5. Admin can create new game categories
6. Users can view existing games
7. Working navbar

### Upcoming Features

1. Edit/Delete functionality
2. Search bar
3. Images

## Technologies Used

The main technologies used for this project are as follows:

1. HTML5 - Used to create the basic code and structure for the website
2. CSS3 - Used to style the elements of the webpage
3. JavaScript - For the logic of some of the elements
4. Flask Framework - Used as the main framework for the website
5. MongoDB - Used to store and retrieve the data created from the website.
6. Python version 3.8.7 - Used for routing and support alongside MongoDB and for interaction between pages
7. JQuery - Used to create elements such as colla[sible menu components
8. Materialize CSS - To provide styling and structure for the elements on the webpage.

## Testing

**User Story Testing**

| User Story | Description | Testing |
|:----------:|:-----------:|:-------:|
| 1.| As a user, I would like to be able to search for specific video games and look at reviews. | |
| 2.| As a user, I want to create an account so I can add my own reviews. | New users are able to create an account from the 'Register' page once the required fields for username and password are filled out correctly. Both fields require input for a user account to be created. The new user is directed to a profile page and is then able to freely navigate the site to view games and create reviews.
| 3.| As a user, I want to log in to my existing account to add or edit my reviews. | |
| 4.| As a user, I want to be able to save my review for other users to view. | |
| 5.| As an admin, I want to add new games to the site for users. | The Admin is able to log in through their user credentials and access the 'Manage Games' page, in which they are able to add, edit, or delete games listed on the website. These changes are then updated on the 'Add Review' page and the home page for all users. |

**functionality Testing**

-- All navigation links have been tested and link to the respective pages correctly.
-- New games added by the Admin user type are displayed on the website correctly.
-- Login and registration authentication works correctly and prevents empty fields from being submitted.
-- When adding a review, empty fields can not be submitted.

## Deployment

The project is deployed using Heroku, with the repository on GitHub.

## Credits

### Content

The content was created by following the Code Institute tutorial for the Flask Task Manager project, and heavily modified by myself to suit my use case.

### Media

### Acknowledgements

-- Code Institute group on slack
