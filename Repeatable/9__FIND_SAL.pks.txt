CREATE OR REPLACE PACKAGE emp_sal AS 
   PROCEDURE find_sal (e_id EMP.empno%type); 
END emp_sal;
