# Child-Attendance-Pickup
A full-stack web app that can sign in/out students with Admin, staff, and parent roles. 

## Initial Planning

#Roles: Parents, staff (teachers), and admin

Parents: Have access to child data, one-time use sign out codes, and class
Staff: Have access to some child/parent data from class and start sign in/out process
Admin: Have access to all child/parent/staff data from all classes. Can add/remove parent accounts. Send sign out codes. Start sign-in/out process. 

#Data

User: name, username, password, Role (parent, staff, admin)
  Parent: contact info
  Staff: classroom
Student: name, classroom, parent(s)
Attendance: Student, Parent, Staff, date, signed in (time), status, signed out (time), reason for sign out
PickupCode: code, Student, Parent, created_time, end_time, verified
AuditLog: user, action, time

#Functions

All: Login
Parent: Bring up one time code
Staff: Start sign-in/out process (search child, ask for code, state reason), look at attendence
Admin: Add/Delete parents/child/staff (CSV file in future), send new one time code, Staff functions
