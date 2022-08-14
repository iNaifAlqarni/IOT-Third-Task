# IOT-Third-Task
POST and GET from database:
In this task we will have a ESP32 with dht11 sensor (temperature & humidity sensor).
we will read the temperature and humidity values and send it to MYSQL database, then we will get data from the database and display the values to a website.
Note: we can collect any type of data from any sensor and send it to the database.

Pre-requisites:
To be able to send and get data from MYSQL database we have to install MYSQL database, you can use XAMPP which i an open-source cross-platform web server.

Explanation Walkthrough:
After installing XAMPP create a folder named "sensors" in xampp path xampp>htdocs

Copy the two files in Task3, insert_temp.php and getSensorValues.php to sensors folder

connect dht sensor to the ESP32 like this circut dht11 circut

Note: use can use any sensor you would like.

Before uploading the code DHT_MYSQL.ino in Task3 folder, make sure to change the ssid and password to your WiFi

In phpMyAdmin, create a database named "esp32", then create a table named "dht" with values shown in below image dht table values

Now power ON the ESP32 and use the index.html and app.css files in Task3 to test it.

Let the ESP32 run for few minutes to send data to MYSQL database, and as you can see database now have temperature and humidity data as shown below: dht data

the website should GET these data from the database and display it (display last added row) as shown below: website get data

