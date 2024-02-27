# Job__Application


## Description
This project is a Job Application API built using Spring Boot. It allows users to perform CRUD operations (Create, Read, Update, Delete) on job applications, with data stored in an H2 database. The API endpoints can be tested using tools like Postman.

## Features
- Create job applications
- Retrieve job applications
- Update job applications
- Delete job applications

## Prerequisites
- Java JDK 8 or higher installed
- Maven installed
- Postman or any API testing tool
- Running the Application
- Clone this repository to your local machine.
- Navigate to the project directory.
- Run the following command to start the application:

## Technologies Used
- Spring Boot
- H2 Database
- Maven (or Gradle) for dependency management
- JUnit for testing

## Usage
- Base URL: http://localhost:8080

### Endpoints
- *POST /jobs*: Create a new job application
- *GET /jobs*: Retrieve all job applications
- *GET /jobs/{id}*: Retrieve a specific job application by ID
- *PUT /jobs/{id}*: Update a job application
- *DELETE /jobs/{id}*: Delete a job application

## Testing
You can test the API endpoints using a tool like Postman.
 *Create a new job application*:
   - Open Postman and select the POST method.
   - Enter the request URL: http://localhost:8080/jobs
   - In the request body, provide JSON data for the job application, such as:
   -  json
   -  {
      - "id":1,
      -	"title": "Software Engineer Needed 12",
      -	"description": "Test Description",
      -	"minSalary": "30000",
      -	"maxSalary": "40000",
      -	"location": "New Jersy"
   -  }
 1 . *Post job applications*:
        
   - Select the POST method in Postman.
   - Enter the request URL: http://localhost:8080/jobs
   - Send the request and verify that you post a list of all job applications stored in the database.
   - Send the request and verify that you receive a successful response with the newly created job application data.
   - ![Post](https://github.com/Muskandwivedi39/Job__Application1/issues/1#issue-2155783091)

     
 2. *Retrieve all job applications*:
   - Select the GET method in Postman.
   - Enter the request URL: http://localhost:8080/jobs
   - Send the request and verify that you receive a list of all job applications stored in the database.
   - ![All Get](https://github.com/Muskandwivedi39/Job__Application1/issues/2#issue-2155808478)

2. *Retrieve all job applications*:
   - Select the GET method in Postman.
   - Enter the request URL: http://localhost:8080/jobs
   - Send the request and verify that you receive a list of all job applications stored in the database.

3. *Retrieve a specific job application by ID*:
   - Select the GET method in Postman.
   - Enter the request URL with a specific job application ID: http://localhost:8080/jobs/{id}
   - Replace {id} with the actual ID of a job application.
   - Send the request and verify that you receive the details of the specified job application.

4. *Update a job application*:
   - Select the PUT method in Postman.
   - Enter the request URL with the ID of the job application you want to update: http://localhost:8080/jobs/{id}
   - Replace {id} with the actual ID of the job application.
   - In the request body, provide the updated JSON data for the job application.
   - Send the request and verify that you receive a successful response with the updated job application data.

5. *Delete a job application*:
   - Select the DELETE method in Postman.
   - Enter the request URL with the ID of the job application you want to delete: http://localhost:8080/jobs/{id}
   - Replace {id} with the actual ID of the job application.
   - Send the request and verify that you receive a successful response indicating that the job application has been deleted.
