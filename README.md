# WebApplication2
han bhae ammar.
sara kaam done hy

yeh rahi sql:
create database dafa

create table Players(
P_id int primary key,P_Name varchar(20),Age int,P_Format varchar(10),Score int)

select * from Players

create table info(
e_id int primary key identity(1,1),
id int,
Update_time varchar(100))

create trigger tb_abc on Players
after insert
as
begin
declare @id int
select @id=P_id from inserted
insert into info values
(@id,'New Player with id = '+CAST(@id as varchar(5))+'is inserted at '+CAST(GETDATE()as nvarchar(50)))
end

insert into Players
values
(1,'Babar Azam',25,'Batsman',4524)

insert into Players
values
(2,'Muhammad Rizwan',32,'Batsman',5634),
(3,'Azhar Ali',32,'Batsman',5634),
(4,'Shaheen Shah Afridi',32,'Batsman',5634)

insert into Players
values
(5,'Azhar Ali',32,'Batsman',5634)

select * from Players

select * from info
