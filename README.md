# CastleBnB - A "Clone" of AirBnB

A full-stack web application that allows users to find and review spots (castles) as well as create and manage them.

## Features

- Authentication and authorization, including signup and login functionality
- View spots on the landing page.
- Create and manage castles (spots), including images.
- Create and manage castle reviews.

## Tech Stack

- Backend:
  - Node.js
  - Express
  - PostgreSQL (for production)
  - Sequelize (for development)
- Front-end:
  - React
  - Redux
  - Redux Toolkit

## Future Goals

- Further polish the styling and clean up code.
- Add additional features, such as: bookings, spot searching, and custom profile pages.
- Normalize state management
- Seperate the spot images from the spots with a model to view and manage all images at once.
- Improve accessability of the website

## Live Site

Feel free to checkout a live version of [CastleBnB here!](https://airbnb-clone-i8gb.onrender.com])

## Screenshots

todo

## Run CastleBnB Locally

1. Clone the repository
`git clone https://github.com/AdamScoggins/CastleBnB.git`

2. Change the working directory
`cd CastleBnB`

3. Install dependencies
`npm run install`

4. Create a .env file in the `backend` directory with the following contents:

    ```plaintext
    DB_FILE=db/dev.db
    JWT_SECRET={insert a new, random token here}
    JWT_EXPIRES_IN=60000
    ```

5. Start the backend server
`npm run dev:backend`

6. Start the frontend server
`npm run dev:frontend`

Once you complete these steps, the backend should be running at `http://localhost:8000` and the frontend at `http://localhost:3000`. Visit the frontend in your browser of choice!

## Technical Implementation Details

The project utilizes Redux Toolkit for managing state. The state is separated into different slices for different features, such as users and spots, which includes the associated reducers, actions, and asynchronous thunks. The project follows a consistent structure for these slices, making it easy to understand and maintain.

All requests to the API utilize custom `csrfFetch` functions, which were created for different HTTP methods. This helps ensure that all requests are secure and protected against CSRF.

I tried my best to design the project logically, with all components and their associated styling located in intuitive directories. The frontend is hosted using Render, along with the backend API and the PostgreSQL database, which includes the CastleBnB schema.

I gave a lot of thought to scalability and maintainability for this project. The use of Redux Toolkit helps to ensure that the state management remains clean and easy to manage, even as the project grows and expands. In the future, I do want to clean up some of the state management.

## Challenges

I faced many challenges creating CastleBnB. Some of which are:

### Deployment with Render

Deploying the project using Render was a steep learning curve, but proved to be a valuable learning experience.

### Time Management and Priorities

Balancing the time spent on learning new technologies, implementing features, and making the project scalable and maintainable was a challenge. However, this helped me grow as a software developer and learn more about my own strengths and weaknesses.

### Learning New Technologies

CastleBnB was built using several technologies that were new to me, including Sequelize, React, Redux, and Redux Toolkit. Learning all of these in such a short time definitely qualifies as a challenge here, and also proved to be a great opportunity for learning.

### Scalability and Maintainability

Scalability and Maintainability were arguably my great challenges. I made more modifications (than I can count) to the project's structure, and refactoring of the code, but this process helped ensure that the project would be easy to manage and expand upon in the future. I do believe this was time well-spent!

### User Experience

I wanted to make sure that the average user would find this website easy to use. I spent a lot of time considering the design and functionality of both the frontend and backend to overcome this challenge because this is, in my opinion, one of the highest priorities for any customer-facing app. Despite these difficulties, I believe that the final result is very intuitive and friendly!

## Code Snippets

todo

## Table of Contents

- [Features](FEATURES.md)

- [React Components List](./frontend/REACT_COMPONENTS.md)

- [Database Schema SQL](./backend/schema.sql)

- [Database Schema Diagram](./backend/schema.png)

- [Frontend Routes](./frontend/REACT_ROUTES.md)

- [API Documentation](./backend/README.md)

- [Redux Store Tree](./frontend/REDUX_STORE_TREE.md)


Feb 11 05:12:17 PM  [eslint]
Feb 11 05:12:17 PM  src/features/spots/SpotPage.js
Feb 11 05:12:17 PM    Line 2:10:  'Link' is defined but never used  no-unused-vars
Feb 11 05:12:17 PM  
Feb 11 05:12:17 PM  src/features/spots/addImage/AddSpotImage.js
Feb 11 05:12:17 PM    Line 44:8:  React Hook useEffect has a missing dependency: 'errors.length'. Either include it or remove the dependency array  react-hooks/exhaustive-deps

Style create spot errors
Empty fields with spaces (trim)
