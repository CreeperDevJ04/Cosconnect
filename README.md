# CosConnect: A Web-Based Social Marketspace and Rental Services for Cosplay Essentials

## 📌 Table of Contents
- [Overview](#overview)
- [Folder Structure](#folder-structure)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Credits](#credits)
- [Technologies Used](#technologies-used)
- [Ownership, Rights, and Legal Notice](#ownership-rights-and-legal-notice)

## Overview
CosConnect is a web-based platform designed to provide an integrated social marketspace and rental management system for the cosplay community in the Philippines. It addresses key challenges such as limited costume accessibility, high acquisition costs, and the absence of secure and organized rental channels. The system combines three core components: a marketplace for buying and selling cosplay items, a rental module with real-time availability and calendar-based scheduling, and a social platform that supports user interaction and community engagement.

This system is developed strictly for academic demonstration, evaluation, and research purposes as part of a Capstone Project.


---

## Folder Structure

This folder contains the **full system** for the Cosconnect project, including:


CAPSTONE-SYSTEM/

├── cosconnect-frontend/ # User website

├── cosconnect-backend/ # API server

├── cosconnect-admin/ # Admin panel

├── database_schema/ # Supabase schema, table query & notes

└── README.md # This file


Each part is modular and communicates via API calls.

---

## Prerequisites

- **Node.js** (v18+ recommended)  
  Download and install from: [https://nodejs.org/](https://nodejs.org/)  
  > After installation, you can check the version with your command prompt:
  ```bash
  node -v
  npm -v
  
  ```
- npm (for installing depedencies)
- Supabase account for database & authentication
- Google OAuth credentials, PayMongo API keys, Email SMTP credentials

---

## Installation

- download the zip file and extract it 
- open the parent folder with your IDE (VsCode should suffice)
- inside the parent folder in your IDE this what you should see
<img width="272" height="146" alt="image" src="https://github.com/user-attachments/assets/f395f54e-b1b4-4d00-97c7-f7bee23c21e1" />

- find the terminal in your IDE and run the following commands

### 1. Backend
```terminal

cd cosconnect-backend
npm i --force

```
- wait for it to finish

### 2. frontend
```terminal

cd ..
cd cosconnect-frontend
npm i --force

```
- same goes here
  
### 3. admin
```terminal

cd ..
cd cosconnect-admin
npm i --force

```
- and here

---

## Usage

**Note: Each project contains a .env.example and .env.local.example file. Copy what's inside .env.example into a .env file and .env.local.example to a env.local file and fill in the required values before running.**

### Creating tables in supabase
- first create an account in supabase
- create your project, once done
- go to sql editor in the left sidebar
- inside the folder database_schema are sql queries to create the tables
<img width="259" height="176" alt="image" src="https://github.com/user-attachments/assets/ba43d58b-0cdf-4241-9113-1063c973c0a4" />

- open the txt files and copy paste them in the supabase sql editor and run it (**Note: you must run all of them in order by number from 1 to 7 to avoid error**)

- once you filled up all the .env and .env.local. go to the frontend folder and find the next.config.ts and inside the file change this values **(do the same for the admin folder)**
<img width="694" height="170" alt="image" src="https://github.com/user-attachments/assets/25fbcce8-bb78-4aa0-84bb-5f12fb311ab7" />

-once done filling up the required values. go to your IDE terminal and run the following

**Navigate to your backend folder (If you haven't already)**
```terminal

cd cosconnect-backend

npm run dev

```
**create new terminal**

<img width="194" height="103" alt="image" src="https://github.com/user-attachments/assets/754e27e9-a729-4434-b5f3-e1cfa9cae56c" />

- then proceed with the following command using that new terminal

**Navigate to your frontend folder**
```terminal

cd cosconnect-frontend

npm run dev

```
**create new terminal again**

- using the another teminal proceed
  
**Navigate to your admin folder**
```terminal

cd cosconnect-admin

npm run dev

```
- go to your browser and search **http://localhost:3000/** for your frontend and wait for it to load, same for the admin search **http://localhost:3001/** and wait for it to load.
- 
  (**Note: the last number in the port of the url inside the http://localhost:3000/ changes depends which folder you run first, the first one you run will have 3000 at the end and the second will have 3001 and vice versa**)

---

## Features

- Role-based authentication and authorization
  
- Supabase-powered database and authentication

- Google OAuth login (optional)

- PayMongo payment integration

- Email and notifications

- Admin dashboard with analytics, user and rental management

- Frontend user interface with Marketspace rental service, calendar-based scheduling, community social platform, messages module.

---

## Credits

This project was developed as a capstone thesis for STI College Novaliches by:

- **Jaerby Quesada** (Lead Programmer) = Responsible for developing and implementing the system.
- **Margaret Catipon** (Project Manager) = Handles project documentation and overall coordination.
- **Mikaela Timajo** (System analyst) = In charge of requirements gathering and system design.
- **kysha Arcillas** (Quality Asssurance) = Conducts system testing and prepares quality documentation.

### Technologies used
- **Backend**: Honojs and nodejs
- **Frontend**: Typecript and tailwind
- **Database**: Supabase
- **Security**: Form validation, encryption
- **Development**: Vscode, Windsurf, git

## Ownership, Rights, and Legal Notice
This repository and all associated materials are the original work of the authors.  

© 2025 Cosconnect Team. All rights reserved.  

Any reproduction, modification, redistribution, or use of this system beyond the scope of academic evaluation and grading is strictly prohibited and may be considered a violation of intellectual property rights and academic integrity policies. Such actions may result in disciplinary measures and/or legal consequences in accordance with applicable laws.

Access to this repository is granted solely for academic review and does not confer any ownership, authorship, or usage rights beyond those explicitly stated.

 
