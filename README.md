# Jobster - a job search tracker

## Objective

To provide a tool that consolidates and streamlines information for the job search in one central location.

## Features

Will keep track of applications/company info, interviews, contacts/recruiters, and also Lessons Learned.

## Tech Stack (front-end and backend)

Front-end will be Vite/React/Redux, with an emphasis on Redux Toolkit and Middleware to communicate with the back-end.

Back-end will be primarily AWS-based - Lambdas, Dynamo DB, API Gateway.

## Dependencies

react redux redux-toolkit axios

## MVP
Phase 1 - Applications and Company Info

## Wireframe

## Data Models
- Company info
  
  -- Company Name
  
  -- Description
  
  -- Website

Example:

`{
    name: 'XYZ Corp.',
    description: 'XYZ Corp. makes the finest widgets in the land.',
    website: 'http://www.xyz.com'
}`
  
- Applications
  
  -- Position
  
  -- Applied
  
  -- Company (Foreign Key)
  
  -- URL
  
- Interviews
  
  -- Date
  
  -- Company (Foreign Key)
  
  -- Note
  
  -- Lessons Learned
  
- Contacts
  
  -- Application
  
  -- Person Contacted
  
  -- Company (Foreign Key)
  
  -- Date
  
  -- Notes
  
- Recruiters
- Lessons Learned
  
  -- Application (Foreign Key)
