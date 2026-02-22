# dbms-program-8

Write a program to generate the numbers using LOOP, FOR LOOP and WHILE LOOP up to the number inputted by user


set serveroutput on;

declare

    n number;
    i number;

begin

    n := &enter_number;

    dbms_output.put_line('using loop');
    i := 1;
    loop
        exit when i > n;
        dbms_output.put_line(i);
        i := i + 1;
        end loop;


    dbms_output.put_line('using while loop');
    i := 1;
    while i <= n loop
        dbms_output.put_line(i);
        i := i + 1;
    end loop;


    dbms_output.put_line('using for loop');
    for i in 1..n loop
        dbms_output.put_line(i);
    end loop;

end;
/
