## **Set-up emonHub**

During the installation the following settings will be prompted for and the default answers can be accepted or edited.

|| Setting | Default value | Enter | Explanation|
| :---: | :--- | :--- | :--- | :--- |
| 1 | RFM12B serial port | /dev/ttyAMA0 |  ||
| 2 | RFM12B radio group | 210 |  |
| 3 | RFM12B frequency (433 / 868 / 915 MHz) | 4 | 4 or 8 or 9 ||
| 4 | RFM12B node ID | 15 | ||
| 5 | RFM12B time sending interval (sec) | 0 | | |
|6|Name of dispatcher|emoncms-local||
|7|Dispatcher protocol|http://|||
|8|Dispatcher endpoint host|localhost|||
|9|Dispatcher endpoint path|/emoncms|||
|10|Dispatcher endpoint API write key|Your API Key|||
|===

After these details have been entered emonHub will be installed and set up for use. 

*note - to change these settings after installation see [configuring emonHub]()*
