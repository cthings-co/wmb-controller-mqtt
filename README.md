# Wireless Modbus Bridge MQTT Examples

Those examples shows how to integrate Wireless Modbus Bridge with python code using MQTT an Wirepas. They provide sample solutions for [Zephyr RTU Server](https://docs.zephyrproject.org/latest/samples/subsys/modbus/rtu_server/README.html) and [F&F le-01mq energy metter](https://www.fif.com.pl/en/usage-electric-power-meters/630-electricity-consumption-meter-le-01mq.html)

## Usage
First install dependencies: `pip install -r requirements.txt`

Example commands to use:

* Device Configuration:
`python configuration_mqtt.py --host <host> --password <password> --gw <gw_id> --cmd <cmd> <cmd_depndent_args>`

* le-01mq example (this example send read voltage command every set period and displays answet in the console):
`python le_01mq_mqtt.py --host <host> --password <password> --gw <gw_id>`

* le-01mq continous mode example (this example configure WMB to automatically send multiple read parameters commands every set interval and displays voltage answer in the console):
`python le_01mq_set_continous_mqtt.py --host <host> --password <password> --gw <gw_id>`

* zephyr RTU server example (this example allows sending commands to the device):
`python zephyr_rtu_server_mqtt.py --host <host> --password <password> --gw <gw_id> --cmd <cmd> <cmd_depndent_args>`

for complete list of the arguments look into the code.




