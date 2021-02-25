# The Game Corner

![Various Devices](https://github.com/CosmicAsad/DCD-Milestone-Project-3/blob/master/static/img/responsive.png)

The Game Corner is a website dedicated to compiling and providing reviews of video games. 
The website allows user input to search for and view information about various video games, as well as allowing them to write their own reviews, to recommend or criticise the respective video game.
Additionally, new games can be added and removed by the admin.
This website is my Milestone Project 3 for the Full Stack Developer course on code institute

---

## User Experience (UX)
The goal of this website is to provide a satisfactory user experience and allow video game fans and critics to write their own opinion pieces on popular video game titles.
The website should allow users to easily log in or register, and search for the video game title they wish to view.
The user should then be able to easily add or edit their reviews as well as view reviews created by other users.

---

### User Stories
1. As a user, I would like to be able to search for specific video games and look at reviews.
2. As a user, I want to create an account so I can add my own reviews.
3. As a user, I want to log in to my existing account to add or edit my reviews.
4. As a user, I want to be able to save my review for other users to view.
5. As an admin, I want to add new games to the site for users.

---

### UX Framework

**1. Strategy**

The Game Corner is a video game review website with front-end and back-end functionality, created using HTML, JavaScript, CSS, Python, Flask, and MongoDB.
The goal is to create a website that is user-friendly and allows users to easily find and review video games.

**2. Scope**

The website is interactive and allows users to unput their own reviews for other users to see, as well as allowing them to edit their content, and search for different games.
The website has CRUD functionality.
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
Once logged in, users are able to click on the main header, which allows them to search for games, and add or edit reviews. They are able to then save the review.
Once the user wishes to end their session, they can click the 'Log Out' option in the menu to return to the home page.

**4. Skeleton**

The skeleton of the website will utilise Materialize for the CSS layout of the pages. A navigation menu will allow users to go to their chosen pages.
The main landing page will function to allow users to select which title they want to review, and provide links to add or edit their own reviews. This minimises the need for different pages for users to visit and provides a seamless experience.
When adding or editing a review, a drop down text input box will open for users to add their text and rating, and save it.
Additional optiions in the navigation menu allow the user to navigate back to their own profile, or to end the session and log out.
This simplifies the number of options for the user and keeps the website easy to use.

**5. Surface**

The surface design of the website will also utilise Materialize CSS to provide a theme and styling for the components of the website.
Google Fonts is used to style the text using the 'Roboto Mono' font, and FontAwesome is used for various icons.
The colour scheme is designed to be visually appealing to the target audience of gamers, and provide clear readability as well as being responsive.

---

### Wireframe

My wireframe was created using the Balsamiq program, and shows the basic layout for the website in desktop as well as responsive formats such as smartphones and tablets.
Notes describing each wireframe are included below each page of the PDF, linked below.
[Wireframe PDF made in Balsamiq](https://github.com/CosmicAsad/DCD-Milestone-Project-3/blob/master/static/wireframes/MS3-wireframe.pdf)

---

## Features

### Existing Features

1. Register functionality
2. Login functionality
3. Log out functionality
4. Profile page
5. Admin can create new game categories
6. Users can view existing games
7. Working navbar
8. Edit/Delete functionality for admin
9. Edit/Delete functionality for users
10. Search bar
11. Images

### Upcoming Features

1. Expand on profile page

---

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
9. Google Chrome browser Developer Tools - Used for testing during development.

All other installed packages are listed in [requirements.txt](/https://github.com/CosmicAsad/DCD-Milestone-Project-3/blob/master/requirements.txt)

### Security

The user authentication uses SHA256 encryption. In addition, blank forms are not able to be submitted to gain access to the site features, as well as only the admin user being able to create, read, update and delete games.

---

## Testing

**User Story Testing**

| User Story | Description | Testing |
|:----------:|:-----------:|:-------:|
| 1.| As a user, I would like to be able to search for specific video games and look at reviews. | The search bar on the home page allows user input, and works for upper and lower case characters. Full words must be typed to find a game that has the word in it's title. If a search query does not return any results, no games will be displayed. |
| 2.| As a user, I want to create an account so I can add my own reviews. | New users are able to create an account from the 'Register' page once the required fields for username and password are filled out correctly. Both fields require input for a user account to be created. The new user is directed to a profile page and is then able to freely navigate the site to view games and create reviews.
| 3.| As a user, I want to log in to my existing account to add or edit my reviews. | Users are able to navigate to the add review page or edit review page from the home page. The add review button navigates the user to a collapsible form where they are able to submit their review, which displays with their username below the respective game. The edit game button is available on existing reviews created by the user, to prevent editing other's reviews. The button directs users to a form that is prepopulated with their existing review. The changes can then be updated and reflected on the main page. The delete review button allows users to remove their review from the site. |
| 4.| As a user, I want to be able to save my review for other users to view. | Users are able to save their reviews to the site and can be viewed without logging in, by all visitors. The reviews are displayed under each respective game title in a collapsible list. |
| 5.| As an admin, I want to add new games to the site for users. | The Admin is able to log in through their user credentials and access the 'Manage Games' page, in which they are able to add, edit, or delete games listed on the website. These changes are then updated on the 'Add Review' page and the home page for all users. |

**Functionality Testing**

- All navigation links, including mobile navigation links have been tested and link to the respective pages correctly.
- New games added by the Admin user type are displayed on the website correctly, and in alphabetical order.
- Login and registration authentication works correctly and prevents empty fields from being submitted.
- The admin user is the only user that is able to access the 'Manage games' link, and therefore the only user able to add new games and images to the site.
- The admin is able to edit and delete existing games.
- New users are directed to the profile page.
- Users can view all games on the home page, and all existing reviews. 
- Users can add a review for any game they choose, and it will display in the user reviews section below that game.
- Users can not edit reviews created by other users.
- When adding a review, empty fields can not be submitted.
- Deleting reviews successfully removes them from the database and site.
- The site is responsive and works on all devices and screen sizes.

- When testing smaller screen sizes using Chrome Developer Tools, the page formatting can display incorrectly. This can be fixed by clearing the cache using Ctrl + shift + r.

**Validation testing**

- HTML code was validated using the W3C Markup Validation Service, with no unexpected errors.
- CSS code was validated using the W3C Markup Validation Service, with no unexpected errors.
- Python code was validated using the [ExtendsClass Python Syntax Checker](https://extendsclass.com/python-tester.html) with no syntax errors found.

---

## Deployment

1. To clone the repository, type the following command into your terminal:
- git clone https://github.com/CosmicAsad/DCD-Milestone-Project-3
2. Change your directory to the cloned directory using the CD command in the terminal.
3. Create an env.py file in the root directoy and set up the following environment variables to link to your MongoDB Atlas:
   - At the top of the file, import os
   - Create the MONGO_URI and SECRET_KEY variables
   - Set the IP and PORT
4. Install the requirements.txt file using: 'pip3 install -r requirements.txt'
5. To create the data schema in your MongoDB Atlas, create a new database called 'games_db', and add 3 collections, with the following documents:
    1. games
        - game_name
        - game_genre
        - game_description
        - game_img
    
    2. reviews
        - review
        - created_by
        - game_id

    3. users
        - username
        - password

6. Run the app using python3 app.py

### Heroku Deployment

To deploy the app using Heroku, use the following steps:

1. Use pip3 freeze > requirements.txt to create a list of the dependencies for the website.
2. Create a Procfile for Heroku using this command: echo web: python app.py > Procfile
3. Use git add -A , git commit -m "(Your commit message)" , and git push , to push these files to your GitHub repository.
4. Navigate to Heroku and log in.
5. Create a new app by navigating to 'New' and 'Create New App'. Enter your app name and select your region and create app.
6. Under the 'Deploy' tab, select 'GitHub - Connect to GitHub'.
7. Enter your repository's name in the input field, and connect once found.
8. To set your environment variables navigate to the 'Settings' tab and scroll down to 'reveal config vars'
9. Add the following variables:


| Key | Value |
|:---:|:-----:|
| IP | 0.0.0.0 |
| PORT | 5000 |
| MONGO_DBNAME | (The name of your MongoDB database) |
| MONGO_URI | (Your MongoURI can be retrieved by going to MongoDB -> Collections -> Connect -> Connect to your application. Here you can use your credentials to generate the URI.) |
| SECRET_KEY | (The secret key is a unique key known only to the developer) |

10. Navigate to the 'Deploy' tab. To enable automatic deployment, scroll down to the 'Automatic Deploys' section.
11. Choose your GitHub branch and enable automatic deployment.

---

## Credits

### Content

The content was created by following the Code Institute tutorial for the Flask Task Manager project as a base, and heavily modified by myself to suit my use case.

### Media

The games and their cover art have been selected by myself, for educational purposes.
Images used are as follows:

1. [Doom: Eternal](https://steamuserimages-a.akamaihd.net/ugc/800992064379440472/9755AC3E97FFDB2A002306C83E2ED2950AFF9EB9/?imw=512&&ima=fit&impolicy=Letterbox&imcolor=%23000000&letterbox=false)
2. [Grand Theft Auto V](https://acclaimmag.com/wp-content/uploads/2013/04/Untitled-1.jpg)
3. [Mario Odyssey](https://www.mobygames.com/images/covers/l/435360-super-mario-odyssey-nintendo-switch-front-cover.jpg)
4. [Nier: Automata](https://www.mobygames.com/images/covers/l/382107-nier-automata-playstation-4-front-cover.jpg)
5. [Pokemon: Sword & Shield](https://gamepreorders.com/wp-content/uploads/2019/06/cover-art-12.jpg)

Google Fonts was used to obtain the free font 'Roboto Mono' [Google Fonts link](https://fonts.google.com/specimen/Roboto+Mono?query=robo&preview.text_type=custom)
FontAwesome 5 was used to provide various icons used throughout the site.

### Acknowledgements

- Code Institute group on slack
- Tutor support team