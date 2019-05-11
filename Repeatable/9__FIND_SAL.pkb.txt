CREATE OR REPLACE PACKAGE BODY emp_sal  AS  
 PROCEDURE find_sal (e_id EMP.empno%type) IS 
   e_sal EMP.sal%TYPE; 
   BEGIN 
      SELECT sal INTO e_sal 
      FROM EMP
      WHERE empno = e_id; 
      dbms_output.put_line('Salary: '|| e_sal); 
      
   END find_sal ; 
END emp_sal ; 


