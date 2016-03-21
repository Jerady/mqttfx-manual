# MQTT.fx 1.0.0
*Rev.1.0*

MQTT.fx aims to be an quick and easy to use desktop tool for MQTT debugging and testing.
Since about 2 years it is continuously extended (and bug-fixed) by [Jens Deters](http://www.jensd.de).

Recently version 1.0.0 was released, including:

* Connection Profiles for different setup of MQTT broker connections
* ad-hoc connections
* publish / subscribe
* username/password authentication 
* SSL/TLS support
* clipboard for predefined messages
* $SYS-Topics / Broker Status (HiveMQ & mosquitto)
* proxy-support
* stored history of last used topics (per profile)
* Scripting support via Nashorn Engine
* logging console
* bundled installers for all platforms
* update check
* Free! (Apache 2.0 license)

![](mqttfx_about.png)

MQTT.fx is the recommended tool for **Amazon Web Services** IoT [quickstart](http://docs.aws.amazon.com/iot/latest/developerguide/verify-pub-sub.html).

Furthermore there is a tutorial by *Lady Ada* to use MQTT.fx as 
[Desktop MQTT Client]( 
https://learn.adafruit.com/desktop-mqtt-client-for-adafruit-io/overview) for **Adafruit.io**.

**Website:** www.mqttfx.org

**Twitter:** @mqtt_fx











## Log
The „Log“ tab shows the logging console.
The same information is also written to the mqttfx.log file located in the application configuration folder.

![](mqttfx_log_1.png)

## Download and Installation
Bundled installation packages for **Mac OSX**, **Windows** and **Linux** are available at [http://www.mqttfx.org](http://www.mqttfx.org).

![](mqttfx_mqttfxorg_1.png)

"Bundled" means, the Java Runtime Environment to run the application is already included by the Installer, so no pre-installed JRE is needed. The bundles JRE is used only to run MQTT.fx. It is not installed on the System.

![](mqttfx_install_1.png)

 
## Updates
The application is checking for available updates during start-up and prompting the user:

![](mqttfx_updates_1.png)

Loadable packages are listed, loaded and installed via the download dialog:

![](mqttfx_updates_2.png)

## About the Author
Jens Deters started with (home-) computing about 25 years ago. During the last 15 years he owned several roles in the IT & Telecommunication sector (Software Developer, Trainer, Consultant, Project Manager and Product Manager).

His major passion is still developing software. Today he works as a Senior IT Consultant and at codecentric in Germany. He regularly blogs about his projects to contribute to the JavaFX- and IoT-Community ([www.jensd.de](www.jensd.de), [www.mqttfx.org](www.mqttfx.org)). Jens is also member of the NetBeans Dream Team.

![](Jens_Deters_cc_profil_center_w250px.jpeg)




