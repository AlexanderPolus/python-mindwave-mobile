The purpose of this project was to connect a RaspberryPi with accompanying vehicular body to a Neurosky Mindwave Mobile headset as an attempt to control the device with the user's thoughts. The python written here parses unencrypted signals from the mindwave mobile and communicates commands to the wheels.

Some scripts to access the data streamed by the **Neurosky Mindwave Mobile** Headset over Bluetooth on Linux.

Requirements:
* [PyBluez](http://code.google.com/p/pybluez/), see their [documentation](http://code.google.com/p/pybluez/wiki/Documentation) for installation instructions :)

Usage in python:

```python
mindwaveDataPointReader = MindwaveDataPointReader()
# connect to the mindwave mobile headset...
mindwaveDataPointReader.start()
# read one data point, data point types are specified in  MindwaveDataPoints.py'
dataPoint = mindwaveDataPointReader.readNextDataPoint()
``` 
