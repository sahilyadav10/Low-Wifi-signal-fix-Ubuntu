1. Open terminal, and type the following lines.
   ```
   git clone https://github.com/lwfinger/rtlwifi_new
   cd rtlwifi_new
   make
   sudo make install
   sudo modprobe -rv rtl8723be
   sudo modprobe -v rtl8723be ant_sel=2
   ```       
2. If the problem persists, follow the next step. If not, skip to Step 4.
3. Type the following line in the terminal in terminal, and hit enter. 
   ```
   sudo modprobe -rv rtl8723be
   sudo modprobe -v rtl8723be ant_sel=1
   ```         
4. Run the following command in the terminal. ** Replace X by 2 if Step 1 worked, else replace X by 1 in the following line. **
   ```
   echo "options rtl8723be ant_sel=X" | sudo tee /etc/modprobe.d/rtlbtcoex.conf    
   ```  
  
