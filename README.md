# V380-Outdoor-Camera-Files
A firmware and Ceshi.ini file for a cheap chinese outdoor cctv unit.

If in doubt, you can contact "V380technical@gmail.com", this repository is a backup for my own personal use, using the wrong firmware could brick your camera.

This image belongs to Banggood and V380
![Image of the camera this works for](https://i.imgur.com/kilub1N.jpg)
This is the link: https://uk.banggood.com/10LED-5X-Zoom-HD-2MP-IP-Security-Camera-WiFi-Wireless-1080P-Outdoor-PTZ-Waterproof-Night-Vision-ONVIF-p-1527199.html

The instructions I was given along with the "AK3918E-V200__V2.6.3.3_2019-11-13" Firmware are as follows:

1. Extract the contense of the zip file to the root folder of your SD card (not into any other folder that may be there).
2. Insert the SD card back into the camera and restart the camera, you should hear "firmware update has started" followed by a short pause and then "firmware update completed".
3. Once the firmware update has been completed, wait for the camera to say "system starting, system startup complete, wifi connected/internet connected" and then power off the camera.
4. Remove the SD card and delete the firmware update files, place the sd card back inside the camera and restart. Your firmware update should be completed.

The ceshi.ini file's instructions are much the same, copying the file to SD root and restarting the camera, except this time the camera will
speak some Chinese once it's finished doing what it's doing you can remove the file from the SD card and restart again.

The ceshi.ini file did not work for me, using incorrect ini file lines will cause the camera to freeze during the update, to fix this
just remove lines from your ini file until it works, or if that's awkward just remove the ini file entirely.

Here are some params I've found online (very few worked for me, use at your own risk):  
  
[CONST_PARAM]  
rtsp=1  
rtspaudio=1  
audio=1  
audiorec=1  
audiorecord=1  
micrec=1  
mic=1  
micrecord=1  
telnet=1  
ssh=1  
onvif=1  
web=1  
webinterface=1  
webif=1  
http=1  
