CREATE TABLE student (
    student_id INT,
    student_name VARCHAR(20),
    major VARCHAR(20),
    PRIMARY KEY(student_id)
);

# NOt NULL, Unique, Default, Auto_increment
#DESCRIBE student;

DROP TABLE student;


#ALTER TABLE student ADD gpa DECIMAL(3,2);

#ALTER TABLE student DROP COLUMN gpa;

SELECT * FROM student;

INSERT INTO student VALUES(
    1,'Jack', 'Biology'
);

INSERT INTO student VALUES(
    2,'Kate','Sociology'
);


INSERT INTO student (student_id, student_name) VALUES(3, 'Claire');
INSERT INTO student VALUES(4, 'Jack', 'Biology');
INSERT INTO student VALUES(5,'Mike','Computer Science');


UPDATE student
SET major = 'Bio'
WHERE major = 'Biology';

UPDATE student
SET major = 'Computer Science'
WHERE student_id = 4;

UPDATE student
SET major = 'Biochemistry'
WHERE major = 'Bio' OR major = 'Chemistry';

UPDATE student
SET student_name = 'Tom', major = 'Undecided'
WHERE student_id = 1;

UPDATE student
SET major = 'Undecided'
WHERE student_id = 3;

DELETE FROM student
WHERE student_id = 5;

DELETE FROM student
WHERE student_name = 'Tom' AND major = 'Undecided';

# Basic Queries

SELECT * FROM student;
SELECT student_name FROM student;
SELECT student_name, major FROM student;

SELECT student.student_name, student.major 
FROM student
ORDER BY student_name DESC;

SELECT student.student_name, student.major 
FROM student
ORDER BY student_id DESC;

SELECT *
FROM student
LIMIT 2;

SELECT *
FROM student 
ORDER BY student_id DESC
LIMIT 2;

SELECT *
FROM student
WHERE major = 'Biology' or student_name = 'Kate';

SELECT student_name, major
FROM student
WHERE major <> 'Chemistry';

-- < , > , <=, >= , <>, AND, OR

SELECT * 
FROM student
WHERE 
