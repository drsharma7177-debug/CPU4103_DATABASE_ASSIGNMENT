CREATE DATABASE IF NOT EXISTS CPU4103_practice;
USE CPU4103_practice;
SHOW DATABASES;
CREATE TABLE Student (
Student_id INT PRIMARY KEY,
First_name VARCHAR(50) NOT NULL,
Last_name VARCHAR(50) NOT NULL,
Email VARCHAR(60) UNIQUE);
SELECT * FROM Student;
INSERT INTO Student (Student_id, First_name, Last_name, Email)
VALUES
 (1, "Seikh", "Mohammad", "seikh@example.com"),
 (2, "Jack", "Smith", "jack@example.com"),
 (3, "Mary" , "Jone", "mary@example.com");
 SELECT * FROM Student;

 INSERT INTO Student
 (Student_id, First_name, Last_name, email)
 VALUES 
 (4, "Sila", "Gautam", "sila@example.com");
 SELECT * FROM Student;
 
INSERT INTO Student ( Student_id, First_name, Last_name, Email)
VALUES (2, "Jack", "Smith", "jack@example.com");
SELECT * FROM Student;
ALTER TABLE Student
ADD Age INT;
SELECT * FROM student;
UPDATE  Student
SET Age = 21
WHERE Student_id = "1";
SELECT * FROM Student;
UPDATE Student 
SET Age = 25 
WHERE Student_id = "2";
UPDATE Student
SET Age = 18
WHERE Student_id = "4";
SELECT * FROM Student;
SELECT * FROM Student
ORDER BY Age  ASC;
SELECT * FROM Student;
CPU4103 - INTRODUCTION TO DATABASE
Project Overview
This repository contains my practical work for CPU4103-Introduction to Database.I have used MYSQL to practice database creation , data manipulation, and querying.The practice database is called CPU4103_Practice, and the current table is Student.
Technologies used;
MYSQL server
MYSQL workbench
SQL
GitHub for version control and project documentation
Work Completed
created  the CPU4103_Practice database
created a student table ,defined student_id, first_name, last_name, email and defined a primary key for Student_id to identify each student
used a unique constraint for email and inserted student records using INSERT INTO
Retrived  records using SELECT FROM
Added age column using ALTER TABLE and UPDAT and SET age
Stored records by age using GROUP BY  like ; SELECT * FROM Student ORDER BY Age ASC;
The query displays all the students records of age in ascending order.
Learning Outcome;
Through this practice i have developed my key understanding of database table , relationship between tables, why constraint is necessary and data normalization and using the queries in MYSQL.




