# Hostel-Database-System
SQL based database management project
<h2>Description:-</h2>
This project is based on HOSTEL MANAGEMENT!!
Hostel management system is the database system to maintain the records related to hostel, it’s information, it’s management, staff and students living in it so that anyone can enquire or access the information about everything related to the hostel. Our model consists of information of following Entity sets:-

<h2>1.HOSTEL :- </h2>it has attributes:-
<ol><li>	Hostel number (primary key) </li>
<li>	Capacity</li>
<li>	Hostel Name</li>
<li>	Vacant Rooms and </li>
Some facility attributes like:-
<li>	Mess ID (Foreign Key)</li>
<li> Sports</li>
<li> Newspaper</li>
</ol> 
<h2>2.SKILLD EMPLOYEE:-</h2> it has attributes:-
<ol>	<li>Name (Composite attribute)</li>
	<li>Employee Id	(primary key)</li> 
	<li>Sex</li>
	<li>Salary </li>
	<li>Age</li>
	<li>Contact number ( multivalued attribute)</li>
<li>Mail_id</li>
<li>Post</li></ol>
It is related to entity set hostel (hostel number) via relation manages .			
<h2>3.Non Skilled EMPLOYEE:-</h2> It consist of attribute:-
<ol><li>	Name (Composite attribute)</li>
	<li>Employee Id	(primary key) </li>
	<li>Sex</li>
<li>	Salary/ wage</li>
	<li>Age</li>
	<li>Contact number ( multivalued attribute)</li>
	<li>Company/Contractor’s name</li>
<li>	Working as</li></ol>
It is related to entity set hostel (hostel number) via relation REPAIRS . 
<h2>4.Visitor record.:-</h2>It is divided into attributes:-	
<ol><li> Record number	(Primary   Key)
<li> Timestamp of arrival</li>
 <li>Timestamp of departure</li>
 <li>Contact no. (Multivalued attribute)</li>
<li>Visitor Name</li>
<li>Hostel number(Visited)</li></ol>
It is related to entity set hostel (hostel number) via relation VISITED .
 <h2>5. Student in-out record:-</h2> It has attributes:-
<ol><li>Record number(Primary Key) </li>
<li>Timestamp of sign out</li>
<li>Timestamp of sign in</li>
<li>Roll number(foreign key)</li></ol>
It is related to entity set STUDENT via relation MAINTAINED FOR .
            		
 
<h2>6.STUDENT:-</h2> It has attributes:-
<li>Roll no.(primary key)</li>
<li>Name (Composite attributes)</li>
<li>Date of birth</li>
<li>Age (derived from dob)</li>
<li>Room no.</li>
<li>Contact no. (multivalued attribute)</li>
<li>Mail ID</li>
<li>Address (Composite attributes)</li></ol>
It is related to entity set Hostel via many to one relationship lives in.
<h2>7.Internet:-</h2> It consists of attributes:-
<ol><li>(Hostel number, Room number)(Primary Key)</li>
	<li>IP Address</li></ol>
It is related to entity set hostel (hostel number) via relation FACILITATES .
To reduce redundancy mess is reduced into 2 normalized tables:-Mess-admin and Mess-menu.
<h2>8.Mess-Admin:-</h2> It consists of attributes:-
		<ol><li>Mess ID(Primary Key)</li>
			<li>Catarer’s name</li>
			<li>Representative</li></ol>
 
<h2>9.Mess-Menu:-</h2> It consists of attributes:-
			<ol><li>(Mess Id,Day,Time)(Primary Key)</li>
			<li>Menu</li></ol>
Both of the sets are related to entity set hostel (hostel number) via relation facilitates .

<h1>THIS DATABASE CONSISTS OF 3 TRANSACTION TABLES:-</h1>
<h2>1. SKILLED Employee Transaction:-
</h2> It consists of attributes:-
		<ol><li>ID_No(Primary  Key)</li>
			<li>Attendence</li>
		<li>Working Days</li>
			<li>Hostel (working at Present)</li></ol>
It is related to entity sets skilled employee via relation update .

<h2>2. SKILLED Employee Transaction:-</h2> It consists of attributes:-
		<ol><li>ID_No(Primary  Key)</li>
			<li>Attendence</li>
			<li>Working Days</li>
			<li>Hostel (working at Present)</li></ol>
It is related to entity sets unskilled employee via relation update .

<h2>3.Student transaction:-</h2>It consists of attributes:-
		<ol><li>Roll number(Primary Key)</li>
		<li>Attendence</li>
		<li>Days in Hostel</li>
			<li>Hostel(living at present) </li></ol>
It is related to entity set student via relation update.
 
<h2>Composite attributes description:-</h2>
<ol><li>1.Name:- it is used in many entity sets and has the following attributes:-
1.First name 
2.Last name</li>
<li>2.Address:- it has following attributes:-
1.House no.
2.Street no.</li>
<li>3.Pin code:- It has following attributes:-
1.City
2.State
3.Country
4.ZIP Code</li></ol>
 
<h2>Stakeholders who have to access  the Database and their needs:-</h2>
As the name specifies “HOSTEL MANAGEMENT SYSTEM” is a database developed for managing various activities in the hostel. The stakeholders for this database are :-
<ol><li>Warden of hostels:To keep the record of personal details of each employee and students of the hostel.</li>
<li>Supervisiors of hostels : Same as Warden’s role.   </li>      
<li>Security Officer : To keep the record of the visitors visiting the hostel, arrival and departure time of a student from the hostel.</li>
</ol>All these people are also the administrator of the database.
<ol>The Administrator can :
<li>  Allot different students to the different hostels.</li>
<li> Control the status of the payment of salaries and other expenses. </li>
<li> Edit the details of the students & modify the student records.</li>
<li> If any administrative authority comes to investigate the hostel’s record (like Director etc.), then the administrator can make them see the proper records.
</li></ol>
