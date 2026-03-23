This Repo has scripts to test motor commands for the Waveshare Rasprover. 
You can run these scripts on Linux, MacOS or Windows as long you install the PySerial Python module. 
```pip install pyserial

For a reference JSON commands for see the Waveshare Wiki:
https://www.waveshare.com/wiki/WAVE_ROVER#JSON_Command_Set

* On the Jetson running Linux, the USB port is usually `/dev/ttyACM0`  
* On MacOS, the USB port is something like `/dev/tty.usbmodem#####`, 
  where you will need to find out the exact file name for `######`.  
* On Windows, usually the USB ports under `COM` ports under Device Manager.  
