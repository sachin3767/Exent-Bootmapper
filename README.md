# Exent-Bootmapper
1. Download Bootmapper client from (windows)https://www.dropbox.com/s/3bn9flirkb49ahz/BootMapperClient.zip?dl=0 or (macOS)https://www.dropbox.com/s/wselndg19ofby85/BootMapperClient.mac.zip?dl=0 and the hex files from this rep or latest version from https://github.com/showjean/ps2avrU/releases
2. Open bootmapper client
3. Hold BACKSPACE key or Short the BACKSPACE (or left split BACKSPACE) on your PCB with a pair of tweezers/paperclip while plugging into a DIRECT usb port 
4. Go to Options, click Firm Up and select the ps2avrGB_NKRO.hex file. Wait for it to finish.
5. Go back to Keymapper, and click Download. If you followed the guide correctly, you'll see mapped keys on all columns and rows.
6. Select Load .hex / .json and select the Exent 65 hex file.
7. Tick Reboot after uploading and select Upload.
8. DONE. You can now remap keys as you want by selecting the specific key above and then selecting the function below. Upload and reboot. 

# Underglow RGB Leds
1. Once you're done flashing, go to Options. 
2. Select Connect
3. Change the number of RGB LEDs to 20
4. Select Rainbow and change the colors in each box. Change options 2, 3 & 4 to different colors  
5. You can configure the brightness, colour and speed transition here. 

# Troubleshooting
The PCB is not recognised in devices. 
1. ensure the backspace is held down prior to connecting the board to the PC/mac
2. check in device manager(windows) or system information(macOS) for HIDBoot when in bootloader mode


Bootmapper Client says it does not recognise ps2avrGB device
1. the incorrect firmware has been flashed to the PCB
2. download the latest version from https://github.com/showjean/ps2avrU/releases
3. confirm it is ps2avrGB_firmware_vX...zip
4. unzip the files and when you select firm up, choose the file that is ps2avrGB_NKRO.hex


Some keys are not recognised - usually backspace, pipe, enter, up arrow, right arrow
1. Culprit is the screw-in stabs at the backspace key is shorting the entire column to ground 
2. Fix: add some sticky tape under the screws, just enough to cover the pads. 
