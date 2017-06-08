# MQTT.fx RELEASE NOTES

## Version 1.5 \(02-05-2017\)

* \[Fixed\] Issue \#151: Muting a Topic now works as expected
* \[New\] Issue \#150: Selected Payload Decoder is now stored in ConnectionProfile
* \[New\] Topics Collector: Topics of all incoming Messages \(except '$SYS'\) are now collected.
* \[New\] 'Retained' messages are now tagged with a 'Retained' badge
* \[New\] 'Dublicate' messages are now tagged with a 'DUB' badge

## Version 1.4.2 \(25-05-2017\)

* \[Fixed\] Issue \#28: Removed current implementation to avoid confusion

## Version 1.4.1 \(02-05-2017\)

* \[Fixed\] Issue \#28: Topics are now activated when re-conneting a persistent session
* \[Fixed\] Scripts error cause is now printed into scripts exec log console

## Version 1.4.0 \(24-04-2017\)

* \[New\] All new HTTP proxy support
* \[New\] Support for custom decoder Add-ons
* \[New\] Issue \#129: Settings: Option to clear/keep messages buffer on broker disconnect
* \[New\] The "Disconnected" dialog was replaced by messages at the top of the main window
* \[New\] ConnectionOptions: auto reconnect
* \[New\] ConnectionOptions: max inflight
* \[New\] Main window size and posistion on close is restored at next app start
* \[New\] Application fonts are now 'Lato Medium' & 'Fira Mono'
* \[New\] Some minor UI style modifications
* \[New\] Issue \#144: NSSupportsAutomaticGraphicsSwitching = true is set in macOS version
* \[New\] Comes with Java Runtime version 1.8.0u131

## Version 1.3.1 \(16-01-2017\)

* \[Fixed\] Issue: wrong style is set when detaching panes
* Improved dark theme

## Version 1.3.0 \(25-11-2016\)

* \[New\] Settings: Option to set buffer sizes \(per topic & received messages\)
* \[New\] Settings: Option to set max characters of logging output console and scripting output console
* \[New\] Settings: Support for dark,light and custom themes
* \[New\] Bundled with JRE 1.8.0\_112
* \[Fixed\] memory leak in logging output console and scripting output console
* \[Fixed\] Issue: autoscroll enable/disable

## Version 1.2.1 \(12-10-2016\)

* \[Fixed\] Issue: display the right number of messages

## Version 1.2.0 \(07-10-2016\)

* \[New\] Payload can now be decoded and exported in JSON format
* \[New\] Topic of received messages can now be copied \(and pasted\)
* \[New\] Eclipse Paho 1.1.0 included
* \[New\] Bundled with JRE 1.8.0\_102
* \[Fixed\] Memory leak in terms of received and published messages
* \[Fixed\] Issue when clearing the received messages buffer
* \[Fixed\] Issue when last choosen import/export location is no longer valid

## Version 1.1.0 \(07-04-2016\)

* \[New\] MQTT.fx now has a new fancy icon: Many thanks to Gerrit Grunwald \(@hansolo\_\)!

* \[New\] All new "Subscribe" tab:
  * New rendering of subscribed topics.
  * New rendering of receivied messages.
  * Support for "autoscroll": Always scroll down to latest recevied message and show the details.
  * Message Payload can now be shown as plain text, hex \(fomatted\) and Base64.
  * Payload can now be saved as raw \(binary\), plain text, hex \(fomatted\) and Base64 encoded.
  * Issue \#75: Added an option to 'mute' topics for temporary 'no-show' received messages \(per topic\)
  * Added experimental support of dumping messages payload.
* \[New\] Issue \#70: Support for import/export of ConnectionProfiles
* \[New\] Issue \#71: Support for import/export of Clipboard Messages \(publish messages\)
* \[New\] Issue \#76: Support for import/export of Topics \(respectively for publish and subscribe\)
* \[New\] Extended Scripting API: publish\(\) and subscribe\(\) now also supports "QoS" and "Retained"
* \[New\] Option to clear Messages Clipboard
* \[New\] Option to clear/keep Messages Buffer on unsubscribe
* \[New\] Several style and rendering improvements
* \[New\] Bundled with JRE 1.8.0\_74
* \[Fixed\] Issues with global application logging

## Version 1.0.0 \(02-12-2015\)

* \[Fixed\] Issue \#64: mqttfx-config.xml gets saturated with hundreds of topic in recentSubscriptionTopics
* \[Fixed\] Issues with System MenuBar on OSX
* \[Fixed\] Issue \#58: Publish not working with 0.0.18
* \[Fixed\] Issue \#60: 0.0.18 and 19beta: Run hangs on quit
* \[Fixed\] Issue \#42: Ubuntu 14.04: Crash when trying to check for updates on launch
* \[Fixed\] \#57: Application crash on startup when found update available.
* \[New\] Issue \#59: Copy a topic in the message view
* \[New\] Bundled with JRE 1.8.0\_66

---

## Version 0.0.18

* \[Fixed\] Issue \#52: subscription didn't work anymore on some OS
* \[Fixed\] Issue \#51, \#50, \#46: SSL/TLS certificate issues
* \[Fixed\] MenuBar issues in OS X
* \[Fixed\] Notification issues
* \[Changed\] Switched to ControlsFX 8.40.10 in respect to JDK 8u60
* \[Fixed\] Issue \#55: Abnormal memory usage: Introducing the option or enable/disable $SYS topics subscription
* \[New\] Issue \#56: A "Generate ClientID" button.

## Version 0.0.17

* \[Changed/New\] Issue \#44: Quick Connect Bar is now available
* \[Fixed\] Issue \#49: connection settings window doesn't fit on my screen
* \[Fixed\] App starting issues: Linux version couldn't locate main class since JDK &gt;=u40 was used.

## Version 0.0.16

* \[Changed/New\] Issue \#14 Now TLS/SSL without client certificate authentication is supported
* \[New\] Issue \#35 Subscribe to $SYS topics is now supported
* \[New\] Improved Error Prevention: Profile Editor now supports validation
* \[Fixed\] Issue \#38 Application crash on startup if one script is wrong
* \[Fixed\] Issue \#37 java.io.FileNotFoundException if CA Certificate only is set

## Version 0.0.15

* \[Fixed\] Issue \#31 Unsubscribe + Disconnect form a Broker doesn't clean messages from the client.
* \[Changed/New\] Bound new Output-Handler to Script execution
  * System.out is not bound to the script console anymore!
  * You should now use "output" instead of System.out in Scripts.
  * e.g.: output.print\("Hello from Script"\);
* \[Changed\] JRE 8 update 45 support
* \[Changed\] Logging:
  * better readable logging format
  * now using sl4j \(with log4j\)

## Version 0.0.14.3

* \[Fixed\] Issue \#27 Disconnection when publishing to a second broker
* \[Fixed\] bug when to show only latest messages
* \[Fixed\] bug when receiving broker status messages

## Version 0.0.14

* Clipboard Messages:
  * Order can now be changed by Drag-and-Drop
  * Can be published instantly by click on Button
  * Changes are now stored immediately
* All new appraoch with topics and messages:
  * Rendering revisited
  * Color of topics can now be customized \(messages are colored accordingly\)
  * Topics can now be unsubscribed by click on "-"
  * Number of received messages per topic is shown
  * Messages also do show the wildcard topics which has matched
  * Only longer payloads are expandable now, one-liner are shown as subject
* Fixed an issue with unrecognized characters in topics
* Support for HTTPS proxy connection options

## Version 0.0.13

* Fixed issues with starting external editor to edit scripts
* Added option to choose whether the default system editor should be use or a custom edit command
* Redesinged Settings Dialog
* Added support for subscribe/unsubscribe to Mqtt-Scripting interface
* Added support Refuel API for application updates

## Version 0.0.12

* improved handling of topics containing wildcards
* now using PAHO 1.0.1
* MQTT version support for 3.1 and 3.1.1
* MQTT version can be set via Connecton Profile \(default: 3.1.1, if not supported by broker: 3.1\)
* introducing "Log"-tab: new tab to capture/show the logging stream.
* changed rendering of messages
* fixed some issues when connect/disconnect/connection lost

## Version 0.0.11-1

* fix for issue\#12: now wildcards topics are working again

## Version 0.0.11

* extended menus:
  * you can now subscribe to all recent topics with one click
  * also unsubscribe from all topics is supported
* improved messages rendering:
  * the payload of received messages is now collabsible.
  * fixed issues with topics/messages coloring
* improved subscribe/unsubscribe:
  * the selection of a subscribed topic sets the value of the topics combobox for e.g. unsubscription
  * topics can be unsubscribed by click on the trash-icon
* filter added to show only the latest received messages
* filter added to show only the latest received messages
* 'show notification'property and "show only latest" property are now stored for each connection profile
* new option to set whether detached tabs should be always on top

## Version 0.0.10

* new MQTT-Message Clipboard
* service menu at publish and subscription panel: now you can clear received messages buffer
* option to copy the message payload to clipboard
* extended logging to mqttfx.log
* added Application Window Icon \(for Windows\)
* now running/bundled with Java 8u20
* updated 3rd-party libs \(ControlsFX 8.20.7\)

## Version 0.0.9

* new Settings Dialog: Font size of messages can now be set to a fixed value or dynamic size depending on message size \(not smaller than 0.6em\).
* via Connection Profile Dialog \(Section General\) and Publish /Subscribe now the history of last topics can be cleared.
* exit Dialog: Option 'Do not ask me again!'
* bugfixes \(typos, usability, layout + style issues\)

## Version 0.0.8

* bugfixes \(typos, usability, layout + style issues\)

## Version 0.0.7

* added scripting support
* setup/re-configuration Tool
* reviewed Connection Profile Editor
* reviewed UI and Style

## Version 0.0.6

* Support for Connection Profiles
  * a Connection Profile contains all information for a certain broker connection \(address, port, Auth/SSL settings, ...\)
* Support for SSL / TLS

**Hint:**

Again the configuration-format has changed, v0.0.6 might conflict with former versions.

In this case just delete \(or rename\) the mqttfx-config.xml.

Windows: \[USER\_HOME\]\MQTT-FX\mqttfx-config.xml

OS X: \[USER\_HOME\]/Library/Application Support/MQTT-FX/mqttfx-config.xml

The new configration is automatically created on next app start.

## 2014-07-26 Version 0.0.5

* tabs are now detachable
* UI polish

## 2014-07-03 Version 0.0.4

* revisited UI \(return of "real" buttons\)
* extended support for $SYS-topics: subscription for mosquitto and Hive MQ can be choosen.
* publish and subcrive/receive are now different tabs
* experimental support for http-proxy \(in respect to @dimaki123\).
* last choosen broker &port is restored at next app start
* updated 3rd party libs \(e.g. using features ControlsFX 8.0.6 now\)
* fixed: publish to topics even if now subscribed \(in respect to @\_efwe\_\)

**Hint:**

  


Configuration-format has changed, v0.0.4 might conflict with former versions.

  


In this case just delete \(or rename\) the mqttfx-config.xml.

  


Windows: \[USER\_HOME\]\MQTT-FX\mqttfx-config.xml

  


OS X: \[USER\_HOME\]/Library/Application Support/MQTT-FX/mqttfx-config.xml

  


The new configration is automatically created on next app start.

  


## 2014-06-14 Version 0.0.3

* added broker status tab to support $SYS topics.

## 2014-05-13 Version 0.0.2

* UI-redesign.

## 2014-05-8 Version 0.0.1 alpha 1

* Initial try-out release.



