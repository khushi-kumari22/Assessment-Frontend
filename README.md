# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.
  
Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

# Yoga Classes Admission Form

Welcome to the Yoga Classes Admission Form project! This application allows users to enroll for monthly yoga classes by submitting their details through a user-friendly form.

## Features

- Age Limit: Participants must be within the age range of 18-65.
- Flexible Batching: Users can choose a batch for a month and switch to a different batch in the following month.
  
## Tech Stack

- Frontend: JavaScript and React 
- Backend: Node.js and Express.js
- Database: Firebase

- Node.js provides the runtime and express js framework is used to build the api with /data and /save

## Entity-Relationship (ER) Diagram:

+----------------------+
| Participants         |
+----------------------+
| id (PK)              |
| name                 |
| email                |
| age                  |
| selected_batch       |  |
+----------------------+


## SQL Table:

CREATE TABLE Participants (
  id INT PRIMARY KEY AUTO_INCREMENT,
  name VARCHAR(255) NOT NULL,
  email VARCHAR(255) NOT NULL,
  age INT NOT NULL CHECK (age >= 18 AND age <= 65),
  selected_batch VARCHAR(20) NOT NULL,
);



