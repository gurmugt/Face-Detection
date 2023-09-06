To set up and run the project, follow these steps:

1) Install the Latest JDK:
Ensure you have the latest version of the Java Development Kit (JDK) installed on your system.

2) Install NetBeans:
Download and install NetBeans, an integrated development environment (IDE) for Java.

Check for Other Databases:
In the Control Panel, go to "Add or Remove Programs" and uninstall any other databases such as Microsoft SQL or MySQL if they are installed.

4) Install Microsoft Visual C++ Redistributable Package:
Install the Microsoft Visual C++ Redistributable Package (vcredist_x86.exe) if needed for your system.

5) Install WAMP Server:
Download and install WAMP Server, then start it to set up a local web server environment.

6) Configure NetBeans Project:
Open NetBeans and create a new Java project. Delete the default package created by NetBeans.

7) Copy Project Files:
Open the project's source code and copy the entire "src" folder (the parent folder of all .java files). Paste it into the "Source Packages" section in NetBeans.

8) Add JAR Files:
Right-click on "Libraries" in NetBeans, select "Add JAR/Folder," and open the "libs" folder that came with the project code. Select all files (CTRL+A) and click "Open."

9) Copy DLL Files (Only for 32-bit Systems):
If you're using a 32-bit system, copy all the .dll files from the "dll" folder that came with the code to the C:\Windows folder.

10) Install Java 3D API:
Install the Java 3D API by running the "java3d_1_5...exe" installer.

Copy DLL Files (Only for 64-bit Systems):
If you're using a 64-bit system, navigate to C:\Program Files\Java\Java3D\bin and copy all DLLs to C:\Windows.

11) Configure MySQL:
Open the Wamp Server system tray icon, click on MySQL, and select "MySQL Console." Enter the following commands:

sql
create database 3dface;
use 3dface;
create table users(UserName varchar(30), Email varchar(50), Phone varchar(10), Password varchar(20));
exit;

12) Verify Database Setup:
Open the Wamp Server system tray icon, click on phpMyAdmin. In the browser, navigate to the "3dface" database. You should see the "users" table to confirm the database setup.

Run the Project:
Finally, run the project in NetBeans to test your setup.
