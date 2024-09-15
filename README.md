# Captured-Moments


# Captured Moments

Captured Moments is a fully responsive, dynamic portfolio website designed to showcase a photography gallery. The site allows users to sign up, log in, and manage photos using a CRUD (Create, Read, Update, Delete) interface, with all information stored in a database. The project emphasizes clean design, responsiveness, and ease of use.

## Table of Contents
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Database Structure](#database-structure)
- [Pages Overview](#pages-overview)
- [Customization](#customization)
- [Contact](#contact)

## Features
- **Responsive Design**: Adapts to various screen sizes including mobile, tablet, and desktop.
- **Photo Gallery**: Flip-on-hover photo cards displaying photographer's name and email ID.
- **User Authentication**: Users can sign up with hashed passwords and log in securely.
- **CRUD Operations**: Add, view, edit, and delete photo details in the gallery.
- **Database Integration**: Stores gallery information, sign-up, and login details.
- **Styled Forms**: Contact forms and CRUD input forms are fully styled with validation.
- **Navigation Consistency**: All pages follow a consistent navigation structure and styling.
  
## Technologies Used
- **Frontend**:
  - HTML5
  - CSS3 (custom and responsive styling)
  - JavaScript (for interactivity and form validation)
- **Backend**:
  - PHP (for form handling and CRUD operations)
  - MySQL (for storing user and gallery data)
- **Color Palette**: The site uses a color palette from Color Hunt with the following colors:
  - `#f7efe5` (background elements)
  - `#e2bfd9`, `#c8a1e0`, `#674188` (accent and button colors)

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/captured-moments.git
   cd captured-moments
   ```
2. Set up the database (refer to the Database Structure section below).
3. Modify the `db_connect.php` file with your database credentials:
   ```php
   <?php
   $servername = "your_servername";
   $username = "your_username";
   $password = "your_password";
   $dbname = "your_dbname";
   ?>
   ```
4. Start a local server (e.g., using XAMPP or WAMP) and navigate to the project directory.

## Usage
1. **Sign Up & Login**:
   - Users must sign up with valid credentials, which are securely stored with hashed passwords in the database.
   - Once logged in, users can access the CRUD operations for the photo gallery.
   
2. **Gallery Management**:
   - Users can upload photos, add photographer details (name and email), and edit or delete photos.
   - The gallery features an interactive photo display with flip cards that show additional information on hover.
   
3. **Contact Page**:
   - Users can submit messages via the dynamic contact form, with form validation ensuring proper input.
   - Contact form details are stored in the database.

## Database Structure
1. **Users Table**:
   - `id`: INT, Auto Increment, Primary Key
   - `username`: VARCHAR(50), Unique
   - `email`: VARCHAR(100), Unique
   - `password`: VARCHAR(255) (stored as hashed values)
   
2. **Photos Table**:
   - `id`: INT, Auto Increment, Primary Key
   - `photo_name`: VARCHAR(100)
   - `photographer_name`: VARCHAR(100)
   - `photographer_email`: VARCHAR(100)

3. **Contact Table**:
   - `id`: INT, Auto Increment, Primary Key
   - `name`: VARCHAR(100)
   - `email`: VARCHAR(100)
   - `message`: TEXT

## Pages Overview
- **Home (index.html)**: 
  The homepage with a large hero section showcasing key site features and an introduction to the gallery.
  
- **Gallery (gallery.html)**: 
  Displays the gallery with flip-on-hover images and photo details.

- **Contact Us (contact.html)**:
  Dynamic contact form with validation and submission via PHP, sending data to the database.
  
- **Login & Signup (login.html, signup.html)**:
  User authentication pages with matching navigation and design.

- **CRUD Section**:
  Available after login. Allows users to add, edit, and delete photo entries in the database.

## Customization
- **Color Scheme**: 
  The website uses a specific color palette. You can adjust these colors in the CSS files to suit your brand.
  
- **Hero Section**:
  The hero section is designed with a height greater than `100vh` for a bold visual impact. You can customize this in the CSS by modifying the `.hero-section` class.

- **Form Styles**: 
  Modify the form widths and button styles as necessary in the `styles.css` file.

## Contact
If you have any questions, feel free to contact the project developer:

**Developer**: [Prashant Khanal]  
