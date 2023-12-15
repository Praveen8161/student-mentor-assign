# Mentor Student Assigning API
## Overview
- API to create a new Student Mentor and Assigning them to each other
- Keep track of mentor assigned to the students previously 
- Can change mentor for students it will be automatically updated to both students and mentors
## Endpoints
- Base URL - ` https://student-mentor-assign-82x1.onrender.com/ `

## API Documentation
 - [Click Here](https://documenter.getpostman.com/view/31335509/2s9YeN1818)

## GET Request - All Students
 - Get All the Students data
 - Request Data Format
     - No parameter required

## GET Request - All Mentors
 - Get All the Students data
 - Request Data Format
     - No parameter required

## GET Request - Students with No Mentors
 - Get All the Students with No Mentors Assigned
 - Request Data Format
     - No parameter required

## GET Request - All the Students of a Particular Mentor
 - Get All the students Assigned to the particular mentor
 - Request Data Format
     - Requires Mentor ID in URL params
     - /mentor/allStudents/ :id

## GET Request - All Old Mentors of a Particular Students
 - Get All the Old Mentor of the particular Student
 - Request Data Format
     - Requires Student ID in URL params
     - /student/oldmentors/ :id

## POST Request - Add New Mentor
 - Add new Mentor to the Database
 - Request Data Format
    {
    "mentor_name": "mongo",
    "course": "Full Stack Development"
    }

## POST Request - Add New Student
 - Add new Student to the Database
 - Request Data Format
    {
    "student_name": "doe",
    "batch": "B51WD2"
    }

## Patch Request - Assign Student to Mentor
 - Update the Students to Mentor and Automatically update or   change the Mentor in Students
 - Request Data Format
 - Requires a Mentor ID
 - Requires a Student ID
 - A single Stduent ID can be in a String or Array
 - Multiple Student ID should be in Array
 - Request Data Format
    {
    "mentor_id": "656f7bc38a851844b6a9a2f1",
    "student_id": ["656f6cdce45d1a291671eb51", "656f6cbde45d1a291671eb49"]
    }

    {
    "mentor_id": "656f7bc38a851844b6a9a2f1",
    "student_id": "656f6cdce45d1a291671eb51"
    }

## Deployed URL
 - [Live Site](https://student-mentor-assign-82x1.onrender.com/)

## Front End Deployed URL
 - - [Live Site](https://spontaneous-pony-3ce76f.netlify.app/) 
