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
### Company info
  
  -- Company Name
  
  -- Description
  
  -- Website

**Example:**

`{ name: 'XYZ Corp.',
     description: 'XYZ Corp. makes the finest widgets in the land.',
     website: 'http://www.xyz.com' }`
  
### Applications
  
  -- Position
  
  -- Applied
  
  -- Company (Foreign Key)
  
  -- URL (URL to job posting, if applicable.)

**Example:**

`{ position: 'Software Developer', applied: '1/11/2024', company: '<company id>', url: 'http://www.jobs.com/1234' }`

### Interviews
  
  -- Date
  
  -- Company (Foreign Key)

  -- POC (Point-of-contact/Person you interviewed with.)
  
  -- Notes
  
  -- Lessons Learned

**Example:**

`{ date: '2/1/2024', company: '<company id>', poc: 'Jane Smith', notes: 'Offered job as Software Engineer 2', lessons_learned: 'Don't wear picasso tie next time.' }`
  
### Contacts
  
  -- Name

  -- Type (Recruiter/Manager/Other)
  
  -- Company (Foreign Key)
  
  -- Notes

  -- Email

  -- Number

**Example:**

`{ name: 'Jane Smith', type: 'Manager', company: '<company id>', notes: '', email: 'smith@biz.com', number: '555-555-5555' }`
  
### Recruiters
### Lessons Learned
  
  -- Application (Foreign Key)
