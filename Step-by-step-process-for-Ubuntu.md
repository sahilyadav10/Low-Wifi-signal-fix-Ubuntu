1. Open terminal, and type the following lines.
   ```
   sudo add-apt-repository ppa:hanipouspilot/rtlwifi
   sudo apt-get update
   sudo apt-get install rtlwifi-new-dkms
   ```         
2. Reboot your system. If the problem persists, follow the next steps.
3. Type the following line in the terminal in terminal, and hit enter. 
   ```
   echo "options rtl8723be ant_sel=2"  | sudo tee /etc/modprobe.d/rtl8723be.conf
   ```         
Now, reboot.                                      
