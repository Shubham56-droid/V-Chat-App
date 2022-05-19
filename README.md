# V-Chat-App
V Chat App is a web based chatting app using PHP , HTML , CSS and JavaScript
Download XAMPP for to view this project on your pc.
In browser search localhost/phpmyadmin and create the table below<br/><br/>
<hr/>
-- 1. create database 'chatapp' <br/>
-- 2. create table 'messages' in database<br/>
-- 3. create table 'users' in database<br/>

-- -------------------------------------------------------

CREATE TABLE 'messages' (
  'msg_id' int(11) NOT NULL,
  'incoming_msg_id' int(255) NOT NULL,
  'outgoing_msg_id' int(255) NOT NULL,
  'msg' varchar(1000) NOT NULL
); 

-- --------------------------------------------------------

CREATE TABLE 'users' (
  'user_id' int(11) NOT NULL,
  'unique_id' int(255) NOT NULL,
  'fname' varchar(255) NOT NULL,
  'lname' varchar(255) NOT NULL,
  'email' varchar(255) NOT NULL,
  'password' varchar(255) NOT NULL,
  'img' varchar(255) NOT NULL,
  'status' varchar(255) NOT NULL
) 



ALTER TABLE 'messages'
  ADD PRIMARY KEY ('msg_id');

ALTER TABLE 'users'
  ADD PRIMARY KEY ('user_id');

ALTER TABLE 'messages'
  MODIFY 'msg_id' int(11) NOT NULL AUTO_INCREMENT;

ALTER TABLE 'users'
  MODIFY 'user_id' int(11) NOT NULL AUTO_INCREMENT;



