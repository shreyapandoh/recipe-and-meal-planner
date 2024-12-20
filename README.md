# Recipe Finder and Meal Planner

A web application that allows users to search for recipes, save their favorite recipes, and plan meals for the week. The app integrates with a third-party recipe API to fetch recipe data, and it features a drag-and-drop meal planner, search functionality with debounce, and performance optimization techniques like throttle.

This project aims to provide an engaging, interactive experience for food enthusiasts and individuals looking to plan their meals in advance while learning and implementing core frontend technologies like React, Redux, and API integration.

## Features

- **CRUD Operations**: Users can save, update, or delete their favorite recipes.
- **API Integration**: Fetches recipe data from the [Spoonacular API](https://spoonacular.com/food-api) or [Edamam API](https://developer.edamam.com/), providing detailed information such as ingredients, instructions, and nutrition facts.
- **Search**: Search recipes by ingredients, cuisine type, or dish name with **debounce** functionality to minimize API requests.
- **Meal Planning**: Drag-and-drop interface for adding recipes to a weekly meal plan (Sunday-Saturday).
- **Debounce**: Optimized search bar that delays API calls, reducing the number of requests as the user types.
- **Throttle**: Throttles meal plan updates to ensure smooth performance when adding/removing recipes in the meal planner.
- **Responsive Design**: Fully responsive UI that adapts to mobile, tablet, and desktop screens.
- **Unit Testing**: Unit tests for components like recipe cards, search functionality, and form validations using **Jest** and **React Testing Library**.
- **Component Testing**: Tests for smaller components, such as recipe cards and buttons.
- **Integration Testing**: End-to-end testing for the flow of searching recipes, saving them, and adding them to the meal plan.
- **UI/UX**: Visually appealing design with interactive features such as recipe cards, a drag-and-drop planner, and a responsive layout for a seamless user experience.

## Installation and Setup

1. **Clone the repository**:
   ```bash
   git clone https://github.com/shreyapandoh/recipe-and-meal-planner.git
2. cd recipe-finder-meal-planner
3. npm install
4. npm start

## Tech Stack

- **Frontend**: React, Redux, React Router
- **Styling**: CSS, Flexbox/Grid, Material-UI (or TailwindCSS if preferred)
- **State Management**: Redux
- **API**: Spoonacular API or Edamam API
- **Testing**: Jest, React Testing Library, Cypress (for integration tests)
- **Other Tools**: Axios (for making API requests)

## Folder Structure

public/
  index.html       # HTML template
src/
  assets/           # Static assets like images, icons
  components/       # All React components (e.g., RecipeCard, MealPlanner)
  redux/            # Redux-related files (actions, reducers, store)
  api/              # API-related functions (to fetch recipe data)
  tests/            # Unit tests and integration tests
  App.js            # Main application component
  index.js          # Entry point of the React app
  styles/           # Global styles and theming


## Future Improvements

- **Add a shopping list** feature to automatically generate a list of ingredients based on the weekly meal plan.
- **User authentication** for saving favorites and meal plans to a backend.
- **Custom recipe creation** where users can submit their own recipes and store them in the app.
- **Meal prep tips** with nutritional analysis for each meal.
