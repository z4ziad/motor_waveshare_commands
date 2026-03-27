This Repo has scripts to test motor commands for the Waveshare Rasprover. 
You can run these scripts on Linux, MacOS or Windows as long you install the PySerial Python module.   
```pip install pyserial```

If you are testing the motors on the Jetson, you do NOT need to unplug the USB cabe connecting it to the ESP32:  
* On the Jetson running Linux, the USB port is usually `/dev/ttyACM0`. Note that the script should be run outside of the IsaacROS-dev Docker container. You need to add the username to the dialout gorup:
```$ sudo usermod -aG dialout $USER```
Then log out and back in again or restart the Jetson. Verify that user is now part of the dialout group:
```$ groups $USER```


If you want to test motors on other OSes, you need to bypass the Jetson Orin Nano. Unplug the USB cable going the ESP32 from Jetson side and plug it into the USB port on computer running MacOS or Windows:  
* On MacOS, the USB port is something like `/dev/tty.usbmodem#####`, 
  where you will need to find out the exact file name for `######`.  
* On Windows, usually the USB ports under `COM` ports under Device Manager.  

For a reference JSON commands for see the Waveshare Wiki:
https://www.waveshare.com/wiki/WAVE_ROVER#JSON_Command_Set
