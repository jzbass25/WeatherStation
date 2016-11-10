# WeatherStation
**Cyberphysical Systems Project**

**Client Program**

Takes data from BMP and DHT sensors, sends it to the Server program via websockets along with the date/time.


Install the Adafruit libaries and the  python SocketIO client v0.5.6 on Pi.


-pip install -U socketIO-client==0.5.6

-Adafruit bmp install- https://github.com/adafruit/Adafruit_Python_BMP

-Adafruit dht install- https://github.com/adafruit/Adafruit_Python_DHT


**Server**

Runs the server to serve the webpage

Using apache, index.html replaces their standard index.html and add /static/ to the same folder. Currently cannot get 'localhost' to work with the index.html so currently need to change ip to raspberry pi's ip.


**Server Program**

Will take data from the client's sensors and then send that data to the webpage that is served by the server.

Run on the server, will need to install gevent/socketIO server (look up to see if server is included in gevent)

-pip install gevent-socketio

-Might use redis for database- if so then install redis.
