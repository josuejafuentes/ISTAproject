create database MyFITNESSAPP
(
drop table if exists workout;
create table userinfo
(
userid int not null identity(1,1)
constraint userid primary key,
first_name varchar(20),
last_name varchar(20),
age int,
users_weight int,
users_height int
);

insert into userinfo(first_name, last_name, age, users_weight, users_height)
values('josue','fuentes',23, 200, 68);

drop table if exists dietplan;

create table dietplan
(
userid int not null identity(1,1)
constraint userid primary key,
diet_type varchar(20),

);

insert into dietplan(diet_type)
values('keto');

drop table if exists users_location;

create table users_location
(
userid int not null identity(1,1)
constraint userid primary key,
city varchar(50),
users_state varchar(50),
zip varchar(50),
country varchar(50)
);

insert into users_location(city, users_state, zip, country)
values('purcellville', 'virginia', '20132', 'USA');

drop table if exists run;
create table run
(
userid int not null identity(1,1)
constraint userid primary key,
miles int,
km int,
run_time int,
seconds int,
time_minutes int,
time_hour int
);

insert into run(miles, km, run_time, seconds, time_minutes, time_hour)
values(30, 15, 30, 20, 40, 1);


drop table if exists workout;
create table workout
(
wid int not null identity(1,1)
constraint wid primary key,
userid int,
monday varchar(20),
tuesday varchar(20),
wednesday varchar(20),
thursday varchar(20),
friday varchar(20),
saturday( varchar(20),
sunday varchar(20)
);

insert into workout(userid, monday,tuesday, wednesday, thursday, friday, saturday, sunday)
values(4, 'chest', 'arms', 'legs', 'back', 'chest', 'arms', 'rest');

drop table if exists body_parts;
create table body_parts
(
wid int not null identity(1,1)
constraint wid primary key,
chest varchar(50),
arms varchar(50),
legs varchar(50),
back varchar(50)
);

insert into body_parts(chest, arms, legs, back)
values('c.wk_1', 'c.wk_2', 'w.wk_1', 'w._wk2');

drop table if exists calisthenics;
create table calisthenics
(
wid int not null identity(1,1)
constraint wid primary key,
wk_1 varchar(50),
wk_2 varchar(50),
wk_3 varchar(50),
wk_4 varchar(50),
wk_5 varchar(50)
);

insert into calisthenics(wk_1,wk_2,wk_3,wk_4,wk_5)
values('push-ups','pull-ups','crunches','sit-ups','planks');

drop table if exists weight_lift;
create table weight_lift
(
wid int not null identity(1,1)
constraint wid primary key,
wk_1 varchar(50),
wk_2 varchar(50),
wk_3 varchar(50),
wk_4 varchar(50),
wk_5 varchar(50)
);

insert into weight_lift(wk_1,wk_2,wk_3,wk_4,wk_5)
values('bench-press','squats','dumbbell-press','tricep-extensions','shoulder-raises');
);