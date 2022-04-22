# Sql-Practice-2


--To craete table
create table Employee(
EId int ,
Ename varchar(50),
salary int,
Mobile varchar(15),
Deptno int);
--To see structure of table
SP_Help Emp;

Insert into Employee(EId ,Ename,Salary ,Mobile,Deptno)
values(101,'Ankit Kumar',18000,'635796422',10),
(102,'Amrit Kuar',9000,'6110079645',20),
(103,'Ansh Kumar',10000,'7135790004',30),
(104,'Chandan Kumar',12000,'7063579600',10),
(105,'Chhavi Kumari',13000,'7660019645',40),
(106,'Deepak Kumar',14000,'8062009645',40),
(107,'Harshit Kumar',15000,'9061000645',30),
(108,'Muskan Sagar',16000,'9860106456',20);

SELECT COUNT(EID),Ename,Salary,Deptno FROM Employee
GROUP BY Deptno
ORDER BY salary DESC;

Select * Into Emp1 from Employee;

SELECT * FROM Employee
WHERE Salary BETWEEN 1000 AND 2000;
