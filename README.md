use students;
show tables;

CREATE TABLE Students (
    StudentID INT PRIMARY KEY,
    Name VARCHAR(50),
    Age INT,
    City VARCHAR(50)
);


INSERT INTO Students (StudentID, Name, Age, City)
VALUES
(1, 'Arun', 20, 'Chennai'),
(2, 'Priya', 21, 'Madurai'),
(3, 'Rahul', 22, 'Coimbatore'),
(4, 'Meena', 19, 'Salem');


SELECT * FROM Students;

SELECT * FROM Students
WHERE City = 'Chennai';


UPDATE Students
SET Age = 23
WHERE StudentID = 3;


SELECT * FROM Students
WHERE StudentID = 3;


DELETE FROM Students
WHERE StudentID = 4;

SELECT * FROM Students;
