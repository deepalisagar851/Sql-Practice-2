
create table Employee( EId int , Ename varchar(50), salary int, Mobile varchar(15), Deptno int);

Insert into Employee(EId ,Ename,Salary ,Mobile,Deptno)
values(101,'Ankit Kumar',18000,'635796422',10),
(102,'Amrit Kuar',9000,'6110079645',20), 
(103,'Ansh Kumar',10000,'7135790004',30), 
(104,'Chandan Kumar',12000,'7063579600',10), 
(105,'Chhavi Kumari',13000,'7660019645',40), 
(106,'Deepak Kumar',14000,'8062009645',40), 
(108,'Harshit Kumar',15000,'9061000645',30),
(109,'Muskan Sagar',16000,'9860106456',20);

SELECT Count(EID),Ename,Salary,Moblie,Deptno FROM Employee
GROUP BY Deptno 
ORDER BY salary DESC; 

Select * Into Emp1 from Employee;

create table Department(EID int,Post varchar(25), Department Varchar(25));
Insert into Department(EID,Post, Department)
values(101,'Manager','HR Management'), 
(102,'TL','CLP'),
(103,'Manager','Survey Management'),
(104,'HR','HR Management'), 
(105,'Project Manager','Task Management'),
(106,'TL','GRS'), 
(107,'TM','DDS'), 
(108,'Assistant Mananger' ,'HR Management'),
(109,'TM','GL Management');

SELECT Employee.(*) 
FROM Employee
INNER JOIN Customers ON Orders.CustomerID=Customers.CustomerID;


SELECT * FROM Employee WHERE Salary BETWEEN 1000 AND 2000;
