# Travel Web Application - Frontend

This repository contains the frontend implementation of a simple traveling website based on the client/server architecture. The website allows users to explore various travel destinations, create an account, add places to their "want-to-go list," and search for travel destinations.

## Introduction

The objective of this project is to provide users with a web application for exploring travel destinations. Users can create accounts, log in, add places to their wishlists, and search for destinations. The website is initially hosted on the local machine and later deployed to Heroku for online access.

## Components

### Users Login (Main Page):

- Registered users can log in using their stored username and password.
- Correct credentials redirect the user to the home page.
- Unregistered users see an error message when attempting to log in.

### User Registration:

- Users can create an account with a unique username and password.
- User information is stored in a MongoDB database.
- Error messages display for duplicate usernames or empty fields.
- After registration, users are redirected to the login page with a success message.

### Home Page:

- Displays destination categories (Beaches, Mountains, etc.).
- Button to view the user's "want-to-go list."
- Clicking on a category redirects the user to that category's page.

### Category Page:

- Shows all destinations within a category.
- Clicking on a destination's name redirects the user to the destination's page.

### Destination Page:

- Contains a description of the destination.
- Embeds a link for a video describing the destination (streamed by the user).
- "Add to want-to-go list" button adds the destination to the user's list in the database.
- Displays an error message if the destination is already in the user's list.

### Want-to-Go List Page:

- Displays destinations added by the user.
- "View Want-to-Go List" button on the home page directs the user to their list.

### Search:

- Search bar in all pages (except registration and login).
- Searches destinations by name.
- Results include "Destination not Found" or a list of destinations containing the search keyword.
- Clicking on a search result directs the user to that destination's page.

## Usage

To run the frontend locally, use "node app.js".
