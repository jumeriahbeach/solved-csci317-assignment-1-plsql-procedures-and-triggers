Download Link: https://assignmentchef.com/product/solved-csci317-assignment-1-plsql-procedures-and-triggers
<br>
<h1>Tasks</h1>

<h2>Task 1. Stored procedure )</h2>




Implement a stored PL/SQL procedure APPLICATIONS to list the applicants and their applications.




The names of applicants must be listed in the descending order of last names of applicants.  The position number and title of a position applied by an applicant must be listed in the ascending order of position number.




Execute the stored PL/SQL procedure APPLICATIONS. A fragment of expected sample printout is given below.




16 Zhi Chao Zhong:

2  Johnny Walker:

1 lecturer

6 professor                                                               14 Ivan TheTerrible:                                                        17 Richard TheLionheart:                                                    …

<strong> </strong>




Implement a solution as PL/SQL stored procedure and save it in SQL script file solution1.sql. Then, process the script and save a report in a file solution1.lst. It is explained in Cookbook, Recipe 2.5 “How to use SQL*Plus client ?”, Step 9 how to create and how to save a report from processing of SQL script.




Your report must include listing of all SQL statement processed. To achieve that put the following SQL*Plus commands:




SET ECHO ON

SET FEEDBACK ON

SET LINESIZE 100

SET PAGESIZE 100

SET SERVEROUTPUT ON




at the beginning of SQL script solution1.sql.

<strong> </strong>

<h2>Task 2. Stored function</h2>

Implement a stored PL/SQL function APPLICANTSKILLS that takes an applicant number (anumber) as a parameter, and finds all the skills possessed by the applicant.




The function must return a string of characters that contains the first and last name of an applicant, skill name and level that the applicant possessed.




Execute the stored PL/SQL function APPLICANTSKILLS for all applicants. A fragment of sample printout is given below:




<ul>

 <li>Harry Potter: C programming 4 Java programming 9 cooking 9</li>

 <li>Johnny Walker: Java programming 9 driving 9</li>

 <li>Mary Poppins: C++ programming 10 Java programming 9</li>

</ul>

painting 5

<ul>

 <li>Michael Collins:</li>

 <li>Margaret Finch: SQL programming 6 6 Claudia Kowalewski: SQL programming 8</li>

</ul>

…




Save your implementation of Task 2 in SQL script file solution2.sql. Then, process the script and save a report in a file solution2.lst. It is explained in Cookbook, Recipe 2.5 “How to use SQL*Plus client ?”, Step 9 how to create and how to save a report from processing of SQL script.




Your report must include listing of all SQL statement processed. To achieve that put the following SQL*Plus commands:




SET ECHO ON

SET FEEDBACK ON

SET LINESIZE 100

SET PAGESIZE 200

SET SERVEROUTPUT ON




at the beginning of SQL script solution2.sql.

<strong> </strong>

<h2>Task 3 Statement trigger</h2>

Implement and comprehensively test a <strong>statement trigger</strong> that verifies the following consistency constraint.




<em>“A position cannot need more than 4 skills”. </em>




When ready save your CREATE TRIGGER statement and all SQL statements that comprehensively test a trigger in a script solution3.sql. Comprehensive testing means that the trigger must reject SQL statements that violate the consistency constraint and accept SQL statements that do not violate the consistency constraint. It is a part of your task to find what SQL statements should be tested. Whenever SQL statement violates the consistency constraint a trigger must return ORA-… error message. Use a procedure RAISE_APPLICATION_ERROR to return ORA-… error message. If SQL statement does not violate the consistency constraint then a trigger must return no messages.




Process SQL script file solution3.sql and save a report from processing in a file solution3.lst.




Your report must include listing of all SQL statement processed. To achieve that put the following SQL*Plus commands:




SET ECHO ON

SET FEEDBACK ON




at the beginning of SQL script solution3.sql.







<strong>                                                                                                                                               </strong>

<h2>Task 4 Row trigger</h2>

Implement and comprehensively test a <strong>row trigger</strong> that verifies the following consistency constraint.




<em>“An applicant cannot apply</em><em> for a position during the last 30 days from his/her the previous application for the same position”.</em>







<u>Hint:</u>

No need to consider the UPDATE event.







When ready save your CREATE TRIGGER statement and all SQL statements that comprehensively test a trigger in a script solution4.sql. Comprehensive testing means that the trigger must reject SQL statements that violate the consistency constraint and accept SQL statements that do not violate the consistency constraint. It is a part of your task to find what SQL statements should be tested. Whenever SQL statement violates the consistency constraint a trigger must return ORA-… error message. Use a procedure RAISE_APPLICATION_ERROR to return ORA-… error message. If SQL statement does not violate the consistency constraint then a trigger must return no messages.




Process SQL script file solution4.sql and save a report from processing in a file solution4.lst.




Your report must include listing of all SQL statement processed. To achieve that put the following SQL*Plus commands:




SET ECHO ON

SET FEEDBACK ON


