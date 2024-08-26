
<h1 align="center">
  MealPlanner
</h1>
<p align="center">
  <img src="image.png" alt="Project Cover Image" width="400"/>
</p>

A web application designed to help users create personalized meal plans based on their dietary needs. Users can input their daily calorie goals and the number of meals to generate a customized meal plan.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Setup Instructions](#setup-instructions)
3. [Usage Guidelines](#usage-guidelines)
4. [Project Architecture](#project-architecture)
5. [Technologies Used](#technologies-used)
6. [Future Enhancements](#future-enhancements)

## Project Overview

The Nutritional MealPlanner allows users to input their calorie goals and the number of meals to generate a meal plan with a breakdown of total macronutrient values (proteins, fats, and carbohydrates). The application also supports downloading the meal plan as a PDF for easy reference.

## Setup Instructions

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/zikotan/MealPlanner.git
   cd MealPlanner
   ```

2. **Install Dependencies:**
   Ensure you have [Composer](https://getcomposer.org/) and [Node.js](https://nodejs.org/) installed, then run:
   ```bash
   composer install
   npm install
   ```

3. **Set Up Environment Variables:**
   Create a `.env` file in the root directory and configure your database settings and other environment variables. Use `.env.example` as a reference.

4. **Generate Application Key:**
   ```bash
   php artisan key:generate
   ```

5. **Run Migrations:**
   ```bash
   php artisan migrate
   ```

6. **Serve the Application:**
   ```bash
   php artisan serve
   ```

7. **Open the Application:**
   Open your browser and navigate to `http://localhost:8000`.

## Usage Guidelines

1. **Login/Register:**
   Create an account or log in with your credentials.

2. **Input Calorie Goals and Meal Number:**
   Enter your desired daily calorie intake and the number of meals you wish to have.

3. **Generate Meal Plan:**
   Click on the 'Generate Plan' button to see a customized meal plan based on your inputs.

4. **Download Meal Plan:**
   Use the 'Download PDF' button to save your meal plan as a PDF file.

## Project Architecture

The project follows the MVC (Model-View-Controller) architecture pattern using Laravel. The main components are:

- **Models:** Represent the database tables and business logic (e.g., Meal, User).
- **Controllers:** Handle requests, process input, and return responses (e.g., MealController, AuthController).
- **Views:** Blade templates used for rendering HTML (e.g., home.blade.php, meal.blade.php).

## Technologies Used

- **Front-End:** HTML, CSS, JavaScript, Bootstrap – For a responsive and interactive UI.
- **Back-End:** PHP with Laravel, JavaScript – For server-side logic, Blade templating, and handling user registration and login functionality.
- **Databases:** MySQL – Managed with migrations for user data; JSON – For storing nutritional information.
- **PDF Generation:** HTML2PDF – For creating PDF meal plans.
- **Tools and Services:** GitHub – For version control; XAMPP – For providing a local development environment with Apache, MySQL, and PHP.


## Future Enhancements

- **Macronutrient Input:** Plan to integrate detailed macronutrient input options for more specific dietary planning.
- **Meal Customization:** Allow users to select and add meals to their personal list, enhancing customization.
- **User Interface Refinements:** Continuously improve the UI based on user feedback to enhance the user experience.


## Laravel Setup Instructions

  For the default Laravel setup instructions, see [Laravel README](Laravel_README.md).
