In this SQL file, I created a new column named bin_col to create bins for a histogram. If the bin value is greater than or equal to max_value or less than min_value, they will be replaced accordingly. 


Example: 

CREATE TABLE TABLE1 
(
  grade NUMBER 
);

insert into table1 (grade) values(-6);
insert into table1 (grade) values(-19);
insert into table1 (grade) values(-2);
insert into table1 (grade) values(8);
insert into table1 (grade) values(15);
insert into table1 (grade) values(4);
insert into table1 (grade) values(13);
insert into table1 (grade) values(7);
insert into table1 (grade) values(9);
insert into table1 (grade) values(11);
insert into table1 (grade) values(-16);
insert into table1 (grade) values(-14);
insert into table1 (grade) values(-9);

Procedure:
begin bin_hist('table1', 'grade', 'bin_grade', 2, 10, -10); end;
