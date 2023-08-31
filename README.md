# IoT_SmartGarden
SmartGarden with Arduino, ESP8266
# EasyGame_FinalProject-Semester-HK222
Language: Js, PHP, MySQL. No frameworks used (because I don't know how to use them :D).
First, you need to install and run the latest version of XAMPP (run as admin), then start the MySQL and Apache servers.

Clone this GitHub repository and place it inside the htdocs folder of the XAMPP directory.

Import the SQL file into MySQL in XAMPP through http://localhost/phpmyadmin.

In your web browser, enter http://localhost/EasyGame, the web page will redirect to the clients.

Login:
  Account: admin@gmail.com
  Password: admin

To connect with Arduino devices in the server, copy the path of the 'getData.php' file in the 'servers/data' folder and replace it in the Arduino code file. Information about IoT devices is detailed in the report.pdf file.

Although the group uses different devices from the ones provided by the university, in theory, the functionalities are the same. The difference is in the implementation in the Arduino code and how it sends APIs to the server. (In the Arduino folder, there are two files named `Demo_Master_PHP.ino` and `Node1.ino`, where `Demo_Master_PHP.ino` is for the intermediate device (also explained in the report). Other groups don't seem to use this device. So, this source code needs many changes in both backend and the device itself if used for another project.

Website Result:

- The `auto` function is not yet fully fixed. After setting it, the threshold values for devices in the database do not automatically update and send back to the device.

- The function to send notifications when thresholds are exceeded is not yet implemented.
