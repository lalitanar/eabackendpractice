# EABackend Practice

## Instruction 

Create all APIs that are listed in the link below.

- **Postman API Document**
  - https://documenter.getpostman.com/view/2345572/UzJQoDVn

- **Postman Collection File**
  - https://github.com/lalitanar/eabackendpractice/blob/7ddbb168ff17356c9e64d1f4276289d09593f67e/EABackend%20Practice.postman_collection.json

## Steps
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
   - Show all courses: `GET http://127.0.0.1:8000/api/eacourses`
     - Body Message:
     ![show all courses](https://github.com/lalitanar/eabackendpractice/blob/1578db239a3bc484f2a52f415770b298d811f5a0/showallcourses.png) 
     
   - Find a course by id: `GET http://127.0.0.1:8000/api/eacourses/3`
     - Body Message:
     ![find by id](https://github.com/lalitanar/eabackendpractice/blob/1578db239a3bc484f2a52f415770b298d811f5a0/findcourseid.png)
     
   - Find by courseId: `GET http://127.0.0.1:8000/api/eacourses/findcourseid/EGCO111`
     - Body Message:
     ![find by id](https://github.com/lalitanar/eabackendpractice/blob/1578db239a3bc484f2a52f415770b298d811f5a0/findcourseid2.png)
     
   - Auth: Insert course: `POST http://127.0.0.1:8000/api/eacourses`
     - Require authentication to access this api.
     - Body Message:
     ![insert course](https://github.com/lalitanar/eabackendpractice/blob/1578db239a3bc484f2a52f415770b298d811f5a0/insertcourse.png) 
     
   - Auth: Update course by id: `PUT http://127.0.0.1:8000/api/eacourses/11`
     - Require authentication to access this api.
     - Body Message:
     ![update courses](https://github.com/lalitanar/eabackendpractice/blob/1578db239a3bc484f2a52f415770b298d811f5a0/updatecourse.png)
     
   - Auth: Delete course by id: `DELETE http://127.0.0.1:8000/api/eacourses/3`
     - Require authentication to access this api.
     - Body Message:
     ![delete by id](https://github.com/lalitanar/eabackendpractice/blob/1578db239a3bc484f2a52f415770b298d811f5a0/deletecourseid.png)
     
   - Auth: Delete course by courseId: `DELETE http://127.0.0.1:8000/api/eacourses/deletecourseid/EGCO111`
     - Require authentication to access this api.
     - Body Message (Success):
     ![delete by courseId when success](https://github.com/lalitanar/eabackendpractice/blob/1578db239a3bc484f2a52f415770b298d811f5a0/deletecourseid2.png)
     
     - Body Message (Fail):
     ![delete by courseId when fail](https://github.com/lalitanar/eabackendpractice/blob/1578db239a3bc484f2a52f415770b298d811f5a0/deletecourseid3.png)
     
   - Register: `POST http://127.0.0.1:8000/api/register`
     - Body Message:
     ![register](https://github.com/lalitanar/eabackendpractice/blob/1578db239a3bc484f2a52f415770b298d811f5a0/register.png)
   
   - Login: `POST http://127.0.0.1:8000/api/login`
     - Body Message (Success):
     ![login](https://github.com/lalitanar/eabackendpractice/blob/1578db239a3bc484f2a52f415770b298d811f5a0/login.png)
     
   - Auth: User: `GET http://127.0.0.1:8000/api/user`
     - Require authentication to access this api.
     - Body Message (Success):
     ![user](https://github.com/lalitanar/eabackendpractice/blob/1578db239a3bc484f2a52f415770b298d811f5a0/user.png)
     
   - Auth: Logout: `POST http://127.0.0.1:8000/api/user`
     - Require authentication to access this api.
     - Body Message (Success):
     ![logout](https://github.com/lalitanar/eabackendpractice/blob/1578db239a3bc484f2a52f415770b298d811f5a0/logout.png)
     
     

    
