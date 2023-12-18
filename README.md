# _11018835_Practical-IA---DCIT205

## Overview
This REST API is developed for the Electronic Medical Record System at the University of Ghana Medical Center (UGMC). It manages patient registrations, encounters, and vital signs submission. This backend is implemented using Node.js, Express, and MongoDB.

## Table of Contents
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [API Endpoints](#api-endpoints)
  - [Patient Registration](#patient-registration)
  - [Start Encounter](#start-encounter)
  - [Submit Patient Vitals](#submit-patient-vitals)
  - [View List of Patients](#view-list-of-patients)
  - [View Patient Details](#view-patient-details)
- [Usage](#usage)


## Getting Started

### Prerequisites
- Node.js
- MongoDB
- Postman (or any API testing tool)

### Installation
1. Clone the repository:

   git clone https://github.com/fake-sage/_11018835_Practical-IA---DCIT205

   2. Navigate to the project directory:

cd emr-system

3. Install dependencies:

npm install

4. Start the MongoDB service on your machine.

5. Run the server:

npm start


## API Endpoints

### Patient Registration
- **POST /patients**
- Registers a new patient.
- **Payload:** `patientId`, `surname`, `otherNames`, `gender`, `phoneNumber`, `residentialAddress`, `emergencyContact` (name, contact, relationship).

### Start Encounter
- **POST /encounters**
- Starts a new encounter for a patient.
- **Payload:** `patientId`, `date`, `time`, `typeOfEncounter`.

### Submit Patient Vitals
- **POST /patients/:patientId/vitals**
- Submits vitals for a patient.
- **Payload:** `bloodPressure`, `temperature`, `pulse`, `sp02`.

### View List of Patients
- **GET /patients**
- Retrieves a list of all registered patients.

### View Patient Details
- **GET /patients/:patientId**
- Retrieves detailed information of a specific patient.

## Usage
- Use Postman or any other API testing tool to interact with the API.
- Ensure the MongoDB server is running before using the application.


