# https-github.com-users-shiva34-projects-1
Student Database Management system :)
The file Data_manage.c contains all the code required.
It uses three structures namely student , instructor , courses which store data 
of each of their object in the text files (students.txt, courses.txt, instructors.txt).

Objects of structure student has the following attribules: 

   rollno  // Its a character array of length 50 used to store the roll number  
   
   name    //Another char array which stores name of student
   
   branch  //enum which take a value from {CSE, EE, ME} 
   
   semester //Stores the semester number 
   
   ncourses  //Stores the total courses taken by student 
   
   courses_codes //2-d dynamically initialized character vector storing codes for all courses taken
   
   
Objects of structure course has the following attributes

    code    // Its a character array of length 50 used to store the course code
    
    name    // Its a character array of length 50 used to store the course name
    
    credits // Stores the course credits
    
    ninstructors //Stores the total instructors teaching in that course
    
    instructor_ids //2-d dynamically allocated array which stores the id's of the instructors teaching in that course
    
    nstudents //Stores the number of students taking that course
    
    student_rollnos // 2-d dynamically allocated array storing roll number of students taking that course
    
    
 Objects of the structure instructor has the following attributes
 
    id   //Character array of length 50 which stores id of that instructor
    
    name //Character array of length 50 which stores name of that instructor
    
    
    ncourses //Stores the number of courses taught by that instructor
    
    courses_codes // 2-d dynamically allocated array storing course codes of courses taught by that instructor
    
The program manages the student details (name and roll number) and maps them to their courses and professors taking the courses.

It stores the data in student.txt, courses.txt and instructor.txt. And maps the three structures together using rollno, id, code.
The program automatically removes any repetition.
This being my very first project and may have fewer comments.
