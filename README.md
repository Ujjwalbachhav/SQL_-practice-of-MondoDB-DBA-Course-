# SQL_-practice-of-MondoDB-DBA-Course-
this is the work which is done in the class




show databases;
 
 create database VIT;
 
 drop database VIT ;
 
 show databases;

create database VIT;
drop database VIT;
use ViT;
create table CSE(
s_id int,
s_name varchar(30),
s_mark int
);
drop table cse;
show tables from VIt;

SELECT 
    *
FROM
    cse;
insert into cse values (1001,'Ram Prasad',99);

ALTER TABLE cse RENAME column 
    s_country TO s_state;
desc cse;
select * from cse;

delete from cse where s_id=1002;

insert into cse values(10153,'Ujjwal',50,'India'),(1003,'Tamilarasan',85,);


UPDATE cse SET s_name ='Vishnu'WHERE s_id=1002;
create database practicel;

 use practice1;
 create table Mech(s_id int,s_name varchar(25));

 START TRANSACTION;
 insert into Mech values (101, 'jayanth');
 SAVEPOINT A;
 update mech set s_id=102 where s_id=101;

 SAVEPOINT B; 
 insert into Mech values (103, 'Karthick');
 select * from mech;
 savepoint c;
 select*from mech;
 rollback to B;
 select * from mech;
 commit;

 CREATE TABLE Worker (

WORKER ID INT NOT NULL PRIMARY KEY AUTO INCREMENT,

FIRST NAME CHAR (25),

LAST NAME CHAR(25),

SALARY INT(15),

JOINING DATE DATETIME,

DEPARTMENT CHAR(25),

A Server Logs,
Options File,
PERFORMANCE,
Dashboard,
Performance Reports,
Performance Schema Setup,
INSERT INTO Worker,

(WORKER ID, FIRST NAME, LAST NAME, SALARY, JOINING DATE, DEPARTMENT)

VALUES,

(001, ontks', 'Arora, 100000, 14-02-2019.00.00),
(002, harika", "Verma, 80000, 14-05-11 09.00.00', 'Adain), 
(003, Vishal", Singhal", 200000, 14-02-26 00.00.00,),
(Singh, 500000, 14-02-28 08.00.00 Adein),
(005, vek, Thati, 500000, 14-06-11 09.00.00", "A"),
(006, Vipul, Diwan, 200009, 14-06-11 49.00.00", "Account),
(007, Satish Kumar, 75000, 14-01-20 500.00 Account),
(on, Geetika", "Chauhan, 30000, 14-04-11 03.00.00 Adain),

SELECT *FROM worker 
WHERE slary  not BETWEEN 100000 AND 200000;
slect first_Name from worker where 

SELECT FROM Worker WHERE SALARY=100000 AND DEPARTMENT = HRS

 SELECT FROM Worker WHERE SALARY > 200000;

 SELECT FROM Worker WHERE SALARY=100008 AND DEPARTMENTHR

 SELECT FROM Worker WHERE SALARY between 100000 AND 200000;

 SELECT FROM Worker WHERE SALARY not between 100000 AND 200000;

 SELECT FROM worker
 WHERE salary BETWEEN 200000 AND 400000
 AND WORKER ID in (1,2,3,4,5);
 desc worker;
 
use org123;
select * from worker;
slecct distinct (department) from worker;

SELECTworker_id , first_name , department ,

CASE

WHEN salary >3000000 THEN 'Rich people'

WHEN salary <= 300000 && salary >=100000THEN 'Middle stage '

ELSE 'poor people'

END

AS People_stage_wise

FROM worker;



