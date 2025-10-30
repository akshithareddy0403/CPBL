Project Title: Helping Hand — The Connection Between Land Pollution and Biodiversity Loss

1. Install Required Software

Install Python 3.8 or above

Install Flask web framework

Install Visual Studio Code (or any IDE of your choice)

Install Arduino IDE (for programming NodeMCU)

Install Firebase account (optional for live data storage)

2. Install Required Python Libraries

Open Command Prompt and run:

     pip install flask pandas sqlite3-binary

3. Setup the Database

Open the file init_db.py

Run it using:

    python init_db.py

This will create a database named ecowatch.db and initialize tables for users and hotspots.

4. Configure Hardware

- Components Used:

- NodeMCU ESP8266

- DHT11 (Temperature & Humidity Sensor)

- MQ135 (Air Quality Sensor)

- Jumper Wires, Breadboard, Power Supply

Steps:

1.Connect DHT11 and MQ135 sensors to NodeMCU GPIO pins.

2.Open Arduino IDE → Load your sensor code.

3.Install necessary libraries:

- DHT.h

- MQ135.h

- ESP8266WiFi.h

4.Upload the code to NodeMCU.

5.Connect to Wi-Fi (SSID and password must be updated in code).

5. Run the Flask Web Application

1.Open the terminal in the project directory.

2.Run:

python app.py

3.Open your browser and go to:
 http://127.0.0.1:5000/

6. Login / Register

Default Admin credentials:

Username: admin01

Password: ecoadmin

You can also register as a new user.

7. Upload Dataset

- Use the Upload CSV option on the dashboard.

- The sample dataset is sample_data.csv.


8. Visualize Data

View pollution hotspots on the map.

Analyze biodiversity loss trends through charts.

Real-time data will update automatically when NodeMCU sends new readings.


9. Alert System

If pollutant levels exceed thresholds:

Local buzzer on NodeMCU is activated.

SMS/Email alerts are triggered via Twilio or Firebase Cloud Messaging.


10. Stop the Project

Press Ctrl + C in the terminal to stop Flask.

Disconnect NodeMCU if no longer in use.






















