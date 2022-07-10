# EABackend Practice

## Instruction 

Create all APIs that are listed in the link below.

**Postman API Document**
https://documenter.getpostman.com/view/2345572/UzJQoDVn


1. Create a new laravel project called "eacourses"
2. Create a database called "eapractice" and connect to the laravel project
3. Create model and migrate migration file that can be used to create the table "eacourses" 
   - field 1: id  (auto increment)
   - filed 2: courseId (string, unique)
   - field 3: courseName (string)
   - field 4: couresCredit (tinyInt, default = 3)
   - field 5: timestamp
   - When you migrate this file to database, Table "eacourse" in database will have 6 fields: id, courseId, courseCredit, created_at, updated_at
   ![eacourse Table](https://github.com/lalitanar/eabackendpractice/blob/2537bb18cc274a303fa5d61f0e3aa6c26395d444/eacourse_table.png)
4. Create the resource file
5. Create the controller file
6. Prepare authentication by using Sanctum and middleware
7. Create these APIs: Create/Read/Update/Delete eacourses
   - Show all courses: GET http://127.0.0.1:8000/api/eacourses
   - Find a course by id: GET http://127.0.0.1:8000/api/eacourses/3
   - Find by courseId: GET http://127.0.0.1:8000/api/eacourses/findcourseid/EGCO111
   - Insert course: http://127.0.0.1:8000/api/eacourses
     - Require Authentication to access this api.
     - Body:
     ![]() 
   - 

    
