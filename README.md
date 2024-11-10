# Plantsy 🌱

Plantsy is a simple plant inventory management app built with React. This app allows users to view, add, edit, and delete plants with ease. It also includes features for searching plants and updating prices in real time. This README will walk you through setting up, using, and understanding the key components of the project.

---

## Table of Contents

1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Technologies Used](#technologies-used)
4. [Installation and Setup](#installation-and-setup)
5. [Folder Structure](#folder-structure)
6. [Component Details](#component-details)
7. [API Endpoints](#api-endpoints)
8. [Running the Project](#running-the-project)
9. [Future Enhancements](#future-enhancements)
10. [Contributing](#contributing)
11. [License](#license)

---

## Project Overview

Plantsy is a responsive web application designed to manage a plant inventory system. Users can add new plants with their name, image, and price, as well as update prices and delete plants from the list. This project demonstrates a practical use of CRUD operations with React.

---

## Features

- **Add New Plant**: A form to add a new plant with details such as name, image, and price.
- **Search Functionality**: Filter plants based on the name.
- **Edit Price**: Update the price of a plant with inline editing.
- **Delete Plant**: Remove a plant from the inventory with a simple click.
- **Responsive Design**: The layout adapts well to different screen sizes.

---

## Technologies Used

- **React**: Frontend library for building the user interface.
- **CSS**: Styling for responsive design.
- **JSON Server**: Mock backend to handle API requests.

---

## Installation and Setup

### Prerequisites

Ensure you have the following installed:

- [Node.js](https://nodejs.org/) (version 14 or above)
- [JSON Server](https://github.com/typicode/json-server) for the backend API

### Steps

1. Clone this repository:

   git clone https://github.com/your-username/plantsy.git

2. Navigate to the project directory:
   cd plantsy
3. Install dependencies:
   npm install
4. Start the JSON Server to simulate a backend:
   json-server --watch db.json --port 3001
5. In another terminal, start the React development server:
   npm start

## Folder Structure

plantsy/
├── public/
│ ├── favicon.ico
│ ├── index.html
│ └── images/
├── src/
│ ├── components/
│ │ ├── App.js
│ │ ├── Header.js
│ │ ├── NewPlantForm.js
│ │ ├── PlantCard.js
│ │ ├── PlantList.js
│ │ └── PlantPage.js
│ ├── index.css
│ └── index.js
├── db.json // Mock data for JSON Server
└── README.md

## Component Details

#### App.js: The main component that includes the Header and PlantPage components.

#### Header.js: Displays the app's title and logo.

#### NewPlantForm.js: Contains a form to add new plants.

#### PlantCard.js: Displays each plant’s details, including image, name, and price. Also includes edit and delete functionalities.

#### PlantList.js: Maps over and renders

PlantCard components.

- **PlantPage.js**: The main page, containing the search bar, new plant form, and plant list.

---

## API Endpoints

- **GET /plants**: Retrieves the list of plants.
- **POST /plants**: Adds a new plant.
- **PATCH /plants/:id**: Updates the price of a specific plant.
- **DELETE /plants/:id**: Deletes a specific plant from the inventory.

---

## Running the Project

To run the app locally, start both the JSON server and the React development server, as described in the installation steps above. The app will be accessible at `http://localhost:3000`, and JSON Server will run on `http://localhost:3001`.

---

## Future Enhancements

- **Add Pagination**: Manage large sets of data with pagination.
- **Filter by Price**: Add functionality to filter plants by price range.
- **User Authentication**: Add authentication for a more personalized experience.

---

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch-name`).
3. Make your changes and commit (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch-name`).
5. Open a pull request.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Happy coding! 😊
