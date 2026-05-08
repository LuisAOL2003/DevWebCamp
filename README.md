📋 Table of Contents

Overview
Features
Tech Stack
Project Structure
Getting Started
Author


🎯 Overview
DevWebCamp is a web application for a web design conference, where visitors can browse the event program, view speaker profiles, purchase tickets online and manage their registrations. The application is built with a custom PHP MVC framework — no Laravel, no frameworks — demonstrating clean architecture and OOP principles.

✨ Features

📅 Event program — Browse conference schedule, talks and workshops
🎙️ Speakers section — Speaker profiles with bio and topic
🎫 Ticket purchasing — Select ticket type and complete payment
👤 User registration & login — Attendee accounts with email confirmation
🔐 Protected dashboard — Manage personal registration details
📧 Email notifications — Automated emails on registration and ticket confirmation
🎨 SASS + Gulp — Compiled CSS with a modern build pipeline


🛠️ Tech Stack

LayerTechnologyBackendPHP 8 (custom MVC framework)FrontendHTML5, CSS3, JavaScript (ES6+)StylingSASS / SCSS compiled with GulpDatabaseMySQLRoutingCustom PHP Router (Router.php)DependenciesComposer (PHP packages)Build ToolGulp 4

📁 Project Structure

DevWebCamp/
├── classes/            # Core framework classes (Router, Email, etc.)
├── controllers/        # MVC controllers (PageController, RegisterController…)
├── includes/           # Shared partials (header, footer, db connection)
├── models/             # Data models with MySQL queries
├── public/             # Publicly accessible files (index.php, assets)
│   ├── build/          # Compiled CSS and JS
│   └── img/            # Images and icons
├── src/
│   └── scss/           # SASS source files
├── views/              # HTML templates (PHP views)
├── Router.php          # Main application router
├── composer.json       # PHP dependencies
├── gulpfile.js         # Gulp tasks for SASS compilation
└── README.md

🚀 Getting Started

Prerequisites

PHP 8.0+
MySQL 8+
Composer
Node.js + npm (for Gulp/SASS compilation)
A local server: Laragon, XAMPP, or similar

Installation

bash# 1. Clone the repository
git clone https://github.com/LuisAOL2003/DevWebCamp.git
cd DevWebCamp

# 2. Install PHP dependencies
composer install

# 3. Install Node.js dependencies
npm install

# 4. Compile SASS to CSS
npx gulp
Database Setup
bash# Create a MySQL database

# Then import the schema (if provided):
mysql -u root -p devwebcamp_db < database/devwebcamp.sql
Configure database connection
Edit includes/database.php (or equivalent config file):
phpdefine('DB_HOST', 'localhost');
define('DB_USER', 'root');
define('DB_PASS', '');
define('DB_NAME', 'devwebcamp_db');
Run the project
Point your local server (Laragon/XAMPP) to the project folder, then open:
http://devwebcamp.test or http://localhost/DevWebCamp/public

👤 Author
Luis Ojeda — Full Stack Developer

🌐 portafolio-luis-ojeda.vercel.app
💼 LinkedIn
🐙 GitHub @LuisAOL2003
