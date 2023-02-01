# facial-recognition-attendance-system-with-flask-api

Allows students to poll their attendance seamlessly using their face cam and faculty to see the attendance sheet and student details

Students entering the system will first be directed to the studentside.html where they caan take their attendance.

Faculty should first login to the system and plugin system for the student so that they can open their webcam.

More into the system 


1.First unzip the folder and keep the contents in a folder called 'nived'.
2.Open the startTheSystem folder and open the main.html file in edit mode and change the hyperlinks in the buttons according to your system path.
3.Install the requirements.txt using pip install -r requirements.txt 

4.Go to mysql workbench and run the following code"CREATE DATABASE IF NOT EXISTS `pythonlogin` DEFAULT CHARACTER SET utf8 COLLATE utf8_general_ci;
USE `pythonlogin`;

CREATE TABLE IF NOT EXISTS `accounts` (
	`id` int(11) NOT NULL AUTO_INCREMENT,
  	`username` varchar(50) NOT NULL,
  	`password` varchar(255) NOT NULL,
  	`email` varchar(100) NOT NULL,
    PRIMARY KEY (`id`)
) ENGINE=InnoDB AUTO_INCREMENT=2 DEFAULT CHARSET=utf8;

INSERT INTO `accounts` (`id`, `username`, `password`, `email`) VALUES (1, 'test', 'test', 'test@test.com');


5.Go to app.py and change the mysql password and host name according to your mysql server details.
4.After installing the requirements open cmd in the project folder and type python app.py ,then open another cmd window in the same folder and type python main.py
5.Now open the startTheSystem folder and run main.html in browser.
6.Now the system starts
7.You will see the are you a student or a faculty window.

FACULTY SIDE

There is a login system and registering system.You can login into the system using test as username and password.

You can see 4 option in faculty side of our website.

Once you press the NEW STUDENT button the python program starts running in a new window .check your taskbar

Give your name and roll number and press capture image.
after thats done press train image to train your image properly
You can press the student details button to see your details getting stored .
Now press plugin system to activate the attendance system.
Now student can go to the website asking whether they are student or faculty. press student
then press take attendance then a python window pops in the task bar .
press track image you will see a notification attendance uploaded with details
The take attendance portal will close in two minutes after the faculty press the plugin system button
Now the faculty can see the students attendance uploaded with the time and date once they press the show attendance button.


