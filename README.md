Sports centre booking system - Squad36
=====

### Group Project for COMP1911 Professional Computing Coursework 1
- **Team Members**: 
  - Ayesha Rahman
  - Natalie Leung
  - Hanmun Hwang
  - Sandra Guran
  - Geeyoon Lim
 
  
The web application is build with python Flask framwork along with SQLite3 database.

The user can see the website without loging in, but to make a booking or buy a membership the user has to login/register.

The manager can register/login and edit, delete facilities, activities and see usage&sales chart. Also only the manager can add new staff mambers.

The employee login works only with the given email and password by the manager for security reasons. The employee can amend user bookings by deleting or making new ones.

For all pages you cannot use the same email twice.

## Requirements
1. Python 3.6, recommending [Anaconda](https://anaconda.org/anaconda/python)

## Setup
1. Install flask and packages
```
$ pip install flask
$ pip install flask-login
$ pip install flask-mail
$ pip install flask-migrate
$ pip install flask-wtf
$ pip install flask-babel
$ pip install flask-cors
$ pip install coverage
$ pip install requests
$ pip install sqlite
$ pip install qrcode
```
2. Database
A database is already filled in with the standard facilities and activities, so there is no need to create a new one.

# Running
1. Run the flask application from the project directory, running on localhost
```
$ flask run
```
2. Open the app in browser: [localhost](http://127.0.0.1:5000/)

# Testing the Unit Tests
```
$ pip install pytest
```
1. Run the flask environment, go into sportsCentre folder and run:
$ pytest unittests.py

## Project Overview
This project focuses on developing a **Sports Management System**, designed to handle the management of facilities, activities, and memberships for a sports center. The system includes features for users to register, manage memberships, book facilities, and participate in various activities.

**Key Features**:
- **User Registration & Login**: Secure user registration and login system.
- **Membership Management**: Users can select different membership plans (monthly or annual) and manage their existing memberships.
- **Facility & Activity Booking**: Users can book facilities and activities, with real-time availability and cart system.
- **Admin Features**: Admins can manage users, facilities, activities, and bookings.

## Tech Stack
- **Back-end**: Python (Flask), SQL
- **Front-end**: HTML, CSS (Bootstrap), JavaScript
- **Database**: SQLite (for local development)
- **Version Control**: Git (using GitHub for collaboration)

## Sprint Details

### Sprint 1: Initial Setup & Planning

**Timeline**: 11th February 2023 - 17th February 2023

**Goals**:
- Finalize project scope and agree on a topic.
- Set up project infrastructure and assign roles.
- Create initial UI mockups.

**Tasks**:
- Chose the **Sports Management System** as the project topic.
- Decided on using **Python Flask** for the back-end, **Bootstrap** for front-end styling, and **SQL** for database management.
- Roles were assigned: Ayesha as team leader, other members distributed across UI, database design, and back-end development.
- Ayesha created an initial UI design prototype, which was reviewed and used as the foundation for the next sprint.

**Outcome**:
- Project repository and environment setup.
- Basic UI mockup ready for further iteration.
- Roles and responsibilities clearly defined.

---

### Sprint 2: Core Feature Development

**Timeline**: 17th February 2023 - 24th February 2023

**Goals**:
- Start implementing core features like user registration, login, and membership management.
- Develop a basic database schema.

**Tasks**:
- Designed the **user registration** and **login** systems.
- Created a database schema for users, memberships, and facilities.
- Built initial pages for **facilities** and **memberships**.
- Began linking the back-end (Flask) with front-end pages (HTML/CSS).

**Outcome**:
- User registration and login systems functional.
- Basic database schema in place, ready for expansion.
- Core pages like facilities and memberships connected to the back-end.

---

### Sprint 3: Advanced Features & Debugging

**Timeline**: 24th February 2023 - 3rd March 2023

**Goals**:
- Implement booking system and cart functionality.
- Test, debug, and refine the system to ensure all core features are functioning.
- Integrate individual contributions into the main codebase.

**Tasks**:
- Developed the **facility and activity booking system** with real-time availability checks.
- Added a **cart system** for users to book and purchase memberships and activities.
- Worked on debugging and fixing issues related to the database, login, and booking flows.
- Merged all individual code into the main branch and solved merge conflicts.
- Improved UI elements for better user experience.

**Outcome**:
- Fully functional booking system with cart integration.
- Debugged core features such as login, registration, and booking.
- Merged and unified codebase for smoother collaboration going forward.

---

### Sprint 4: Final Testing & Polishing

**Timeline**: 3rd March 2023 - 9th March 2023

**Goals**:
- Finalize all features and complete remaining tasks.
- Conduct extensive testing for stability and performance.
- Polish the UI and ensure the site is responsive.

**Tasks**:
- Completed **final testing** for login, registration, and booking processes.
- Improved the design of pages such as the **membership**, **facilities**, and **user profile**.
- Refined the **database structure** to handle different membership types and activities.
- Finalized and polished the **user interface** for responsiveness and usability.

**Outcome**:
- Project ready for deployment with all major features implemented and tested.
- Refined UI for a professional, easy-to-navigate experience.
- Bug-free core functionality across all user interactions.

---

## Installation and Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/sports-management-system.git
   ```

2. Navigate to the project directory:
   ```bash
   cd sports-management-system
   ```

3. Install the required Python packages:
   ```bash
   pip install -r requirements.txt
   ```

4. Set up the database:
   ```bash
   flask db init
   flask db migrate
   flask db upgrade
   ```

5. Run the application:
   ```bash
   flask run
   ```

6. Access the application at `http://localhost:5000`.

## Future Enhancements
- **Implement Payment Integration**: Add payment options for memberships and activity bookings.
- **Extend Admin Features**: Provide advanced admin controls for facility and activity management.
- **Improve Search Functionality**: Enhance search for better user experience across facilities and activities.
