Einführung
=======

Message Queue Telemetry Transport (MQTT) hat sich, bereits 1999 von IBM entwickelt, inzwischen zu einem quasi Standard der Kommunikationsprotokolle für M2M bzw. das Internet of Things (IoT) entwickelt.
Eclipse Paho stellt in diversen Sprachen Client-Implementierung zur Kommunikation mit den MQTT-Kommunikationszentralen, den so genannten Brokern (z.B. mosquitto, HiveMQ, RabbitMQ, ActiveMQ), zur Verfügung. 
MQTT.fx ist ein auf JavaFX und Paho basierendes Werkzeug für das Testen von MQTT Kommunikation.

Ganz allgemein betrachtet ist MQTT ein asynchrones, TCP basiertes Client/Broker Publish/Subscribe Protokoll. Dabei haben Nachrichten haben einen nur etwa 2 Byte grossen Header und der Rest ist Payload, wobei es keine Rolle spielt, ob dieser z. B. reiner Text oder Binärcode ist.

Eine Message Queue hat einen eindeutigen Namen („topic“). Dabei können Queue Namen auch mit „/“ getrennt werden und damit Hierarchien abbilden, z. B. „home/outdoors/garden/terrace/lights“. An einer solchen Queue können sich Clients zum Nachrichtenempfang bestimmter Topics anmelden („subscribe“) und Nachrichten, z.B. mit Sensorwerten, die an diese Topics gesandt („publish“) werden, empfangen. 

Projekte und Systeme, die auf MQTT aufbauen, können über die Konsole getestet werden. Der Open Source Broker mosquitto bringt hier beispielsweise die Commandline-Tools „mosquitto_pub“ und „mosquitto_sub“ mit, mit deren Hilfe man Nachrichten senden und empfangen kann.

Wer es aber grafisch, komfortabler und wiederverwendbar bevorzugt, kann hier auch die JavaFX basierte Desktopanwendung MQTT.fx einsetzen. Das Tool wird seit etwa 2 Jahren beständig von mir weiterentwickelt und stellt bisher folgende Funktionen zur Verfügung:




