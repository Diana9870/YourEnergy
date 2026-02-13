# Your Energy

Your Energy is a modern web application for finding exercises and supporting a healthy lifestyle, created as a coursework. The project demonstrates practical skills in working with Vanilla JavaScript (ES6+), integrating with external APIs, and developing a fully responsive interface for Mobile, Tablet, and Desktop.

The main goal of the application is to provide users with a convenient catalog of exercises with the ability to filter by muscle groups, body parts and equipment, as well as quick access to detailed information about each exercise.

## Key features

Quote of the Day — daily inspiration that is automatically loaded from the API on each visit.

Filtering — switch between categories (Muscles, Body Parts, Equipment).

Exercise Catalog — view cards with ratings and key features.

Details — modal window with full description, video (if available) and the ability to rate.

Search — finding exercises by keywords.

Rating system — the ability to leave a rating via PATCH request.

Subscription — a form to receive updates by email.

Pagination — convenient navigation through a large list of exercises.

## Technology stack

Language: JavaScript (ES6+)

Builder: Vite — fast development and optimization

Styling: CSS (Flexbox, Grid, responsive layout)

API: YourEnergy Swagger API

HTML Modularity: Using Partials

Architecture and Code Organization Rules

The project is built on the principles of a clean modular structure without the use of heavy frameworks.

## Basic rules:

All API requests are placed in separate files (/js/api/).

All rendering functions are located separately (/js/rendering/).

All event listeners are placed in main.js.

Each event handler is a separate file in /js/eventHandlers/ (1 file = 1 handler).

CSS variables from variables.css are used.

Common styles and classes are in styles.css.

Large blocks are divided into separate components (partials).

## Event handler logic:

Sets the loader (if necessary).

Clears the previous state.

Makes a request to the API (async/await).

Uses try...catch for error handling.

In case of success, it calls the rendering function.

In case of error, it shows a message via the notification module.

Turns off the loader.

## Main Flow

Listeners (main.js) intercept events.

Event Handlers (/js/eventHandlers/) process logic and call APIs.

API functions (/js/api/) receive data from server endpoints.

Render functions (/js/rendering/) display data in the interface.

## Project Structure

src/index.html — home page

src/favorites.html — favorite exercises page

src/partials/ — HTML components (header, footer, hero, etc.)

src/css/ — project styles

src/main.js — JavaScript entry point

public/ — static resources

## Installation

To install dependencies, run:

npm install
