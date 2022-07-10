# EABackend Practice

## Instruction 

Create all APIs that are listed in the link below.

**Postman API Document**
https://documenter.getpostman.com/view/2345572/UzJQoDVn


1. Create a new laravel project called "eacourses"
2. Create a database called "eapractice" and connect to the laravel project
3. Prepare migration file that can be used to create the table "eacourses" 
   - field 1: id  (auto increment)
   - filed 2: courseId (string, unique)
   - field 3: courseName (string)
   - field 4: couresCredit (tinyInt, default = 3)
   - field 5: timestamp
   - When you migrate this file to database, Table "eacourse" in database will have 6 fields: id, courseId, courseCredit, created_at, updated_at

    
