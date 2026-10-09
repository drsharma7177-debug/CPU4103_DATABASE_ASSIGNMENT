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




