# Ingeteam-ingecon-homeassistant-modbus
Allows to read ingecon inverter parameters from homeassistant

These are the necessary files to add to your homeassistant configuration to read the parameters of the inverter. For this you need to have configured your configuration.yaml in a split way ("Splitting up the configuration"). If this is not your case, you need to add the code of each file inside "configuration.yaml" under its section.

For it to work correctly you only need to have the ingecon inverter firewall open for the "modbus tcp" part and include the IP of your inverter in the modbus.yaml file. After restarting "homeassistant" the new entities will appear.

The parameters shown by the ingeteam ingecon inverter are only parameters related to real-time data. That is why sensors have been added with the integrations platform and thus have a history of the accumulated amounts, which, according to my tests, is quite accurate.
