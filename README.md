# Arduino_MQTT

# Run json server for receice of board 
json-server --watch data.json -H 192.168.0.18 -p 3000

# Run main.py

# must rub server MQTT first by
mqtt % mosquitto -c mosquitto.conf -v

# For Check valur from sensor
mosquitto_sub -i node_01 -h 192.168.0.18 -t "led or dht11"

