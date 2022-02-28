# Spring-Data-JPA-Relationships

Postman commands:

# Create subject
POST http://localhost:8080/subjects

{
    "enrolledStudents": [],
    "name": "Science"
}

# Create student
POST http://localhost:8080/students

{
    "name": "Zoki"
}

# Create teacher
POST http://localhost:8080/teachers
{
    "name": "Krešimir Sučević Međeral"
}

# Get students
GET http://localhost:8080/students

# Get subjects
GET http://localhost:8080/subjects

# Add student to subject(subject id 2, students id 5)
PUT http://localhost:8080/subjects/2/students/5

# Add teacher to subject (class id 2, teacher id 2)
http://localhost:8080/subjects/2/teacher/2