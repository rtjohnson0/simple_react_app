# Cloverhound Interview Challenge

This project is a simple React application that allows users to enter their name, submit the form, and receive a predicted age based on the name using the Agify.io API. The app also keeps track of previous searches and allows users to clear the search history.

## Features

- User can input their name and submit the form to get a predicted age.
- Uses jQuery to make a network request to the Agify.io API.
- Displays the predicted age.
- Stores and displays a list of previous searches.
- Allows users to clear the search history.

## Technologies Used

- React
- jQuery
- Agify.io API
- Babel
- CSS for styling

## Getting Started

### Installation

1. Clone the repository:

2. Open the `index.html` file in your preferred web browser to view the application.

### Usage

1. Enter a name in the input field.
2. Click the "Submit" button to get a predicted age.
3. The predicted age will be displayed below the form.
4. Previous searches will be displayed in a list.
5. Click the "Clear History" button to clear all previous searches.

## Code Overview

### Components

- **UserNameInput**: A functional component for the input field where users enter their name.
- **PredictedAgeDisplay**: A functional component to display the predicted age for a given name.
- **PredictedAgeList**: A functional component to display a list of previous searches and their predicted ages.
- **App**: The main component that manages the state and handles form submission and data fetching.

### App Component

- **State**:
  - `userName`: Stores the current input name.
  - `predictedAges`: Stores the predicted ages for each searched name.
  - `error`: Stores any error message.

- **useEffect**:
  - Updates `localStorage` with the `predictedAges` state whenever it changes.

- **handleSubmit**:
  - Handles the form submission, makes an AJAX request to Agify.io, and updates the state with the predicted age.

- **handleClear**:
  - Clears the search history and updates `localStorage`.

### CSS Styling

- Centered layout with a background image.
- Card component for form and result display.
- Styled buttons and error messages.

## Running the Project

1. Clone the repository and navigate to the project directory.
2. Open the `index.html` file in a web browser.

## Repository Structure

- `index.html`: The main HTML file.
- `style.css`: The CSS file for styling the application.
- `README.md`: This README file.


## Conclusion

This project demonstrates the use of React for building a form, handling state, making network requests with jQuery, and managing local storage. It provides a simple yet effective way to get a predicted age based on a user's name using the Agify.io API.
