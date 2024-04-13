IMPLEMENTATION OF  PL/SQL USING CONDITIONAL 
STATEMENTS  
 
AIM: 
To implement the conditional selection statement in PL/SQL block. 
ALGORITHM: 
STEP 1: Start the program. 
STEP 2: Create the PL/SQL Block with necessary blocks. STEP 3: Declare the necessary variable in the declaration section STEP 4: write the main program logics in the begin block. 
STEP 5: if you want to access the table use the SQL statement. 
STEP 6: if you want to solve any exception, write the exception name with WHEN statement  
STEP 7: Execute the PL/SQL block. 
STEP 8: Give the input values or validate the information from the tables.  
STEP 9: Stop the program. 
 
The PL/SQL stands for Procedural Language extensions to Structured Query Language. Basically, SQL is used to perform basic operations of creating a database, storing data in the database, updating data in the database, retrieving the stored data of database, etc, whereas PL/SQL is a fully Structured Procedural language which enables the developer to combine the powers of SQL with its procedural statements. 
PL/SQL Block 
In a PL/SQL program, code is written in blocks. Each PL/SQL block has 3 sections, which are: 
1.	Declare section 
2.	Begin section 
3.	Exception section 
Followed by END statement at the end 
PL/SQL Block 
PL/SQL block creates the structured logical blocks of code that describes the process to be executed. Such a block consists of SQL statements and PL/SQL instructions that are then passed to the oracle engine for execution. PL/SQL block consists of the following four sections: 
•	DECLARE Section: 
PL/SQL code starts with a declaration section in which memory variables and other oracle objects like cursor, triggers etc can be declared and if required can be initialized as well. Once declared/initialised we can use them in SQL statements for data manipulation. As it is not necessary that we would require variables etc in every PL/SQL code, hence this section is an optional section. 
•	BEGIN Section: 
This section contains the SQL and PL/SQL statements that are required to be executed and contains the main logic. This section is responsible for handling the data retrieval and manipulation, may be working with branching, can use looping and conditional statements, etc. 
•	EXCEPTION Section: 
This section is optional. It is mainly used to handle the errors that may occur between BEGIN and EXCEPTION sections. 
•	END Section: 
This section is the indication of the end of the PL/SQL block. 
PL/SQL Conditional Statements 
Decision making statements are those statements which are in charge of executing a statement out of multiple given statements based on some condition. The condition will return either true or false. Based on what the condition returns, the associated statement is executed. 
For example, if someone says, If I get 40 marks, I will pass the exam, else I will fail. In this case condition is getting 40 marks, if its true then the person will pass else he/she will fail. 
This can be logically implemented in PL/SQL block using decision making statements. 
The decision making statements in PL/SQL are of two types: 
1.	If Else statements 
2.	Case statement 
Let's see them all one by one with examples. 
PL/SQL: if Statement 
The if statement, or the if...then statement can be used when there is only a single condition to be tested. If the result of the condition is TRUE then certain specified action will be performed otherwise if it is FALSE then no action is taken and the control of program will just move out of the if code block. 
Syntax: 
if <test_condition> then 
	 	body of action 
end if; 
PL/SQL: if...then...else statement 
Using this statement group we can specify two statements or two set of statements, dependent on a condition such that when the condition is true then one set of statements is executed and if the condition is false then the other set of statements is executed. 
Syntax: 
if <test_condition> then  	statement 1/set of statements 1 else 
	 	statement 2/set of statements 2 
end if; 
PL/SQL: if...then...elsif...else statement 
It is used to check multiple conditions. Sometimes it is required to test more than one condition 	in 	that 	case if...then...else statement 	cannot 	be 	used. 	For 	this purpose, if...then...elsif...else statement is suitable in which all the conditions are tested one by one and whichever condition is found to be TRUE, that block of code is executed. And if all the conditions result in FALSE then the else part is executed. 
In the following syntax, it can be seen firstly condition1 is checked, if it is true, the statements following it are executed and then control moves out of the complete if block but if the condition is false then the control checks condition2 and repeats the same process. If all the conditions fail then the else part is executed. 
Syntax: 
if <test_condition1> then 
	 	body of action 
elsif <test_condition2>then 
	 	body of action 
elsif<test_condition3>then  	body of action 
... 
... 
... 
else 
	 	body of action 
end if; 
PL/SQL: Case Statement 
If we try to describe the case statement in one line then, then we can say means "one out of many". It is a decision making statement that selects only one option out of the multiple available options. 
It uses a selector for this purpose. This selector can be a variable, function or procedure that returns some value and on the basis of the result one of the case statements is executed. If all the cases fail then the else case is executed. 
Syntax: 
CASE selector  	when value1 then Statement1;  	when value2 then Statement2; 
	 	... 
	 	... 
 	else statement;
end CASE; 
