# Arduino_MQTT

# Run json server for receive of board 
json-server --watch data.json -H 192.168.0.18 -p 3000

# Run main.py

# must run server MQTT first by
mqtt % mosquitto -c mosquitto.conf -v

# For Check value from the sensor
mosquitto_sub -i node_01 -h 192.168.0.18 -t "led or dht11"

