<img align="right" src="https://visitor-badge.laobi.icu/badge?page_id=papercodeIN.BananaPi" height="20" />

# Banana Pi
 
---
<p align="center">
  <span style="font-size: 1.1em; color: #FFD700; font-weight: bold;">✨ Enjoying this project? Support our work! ✨</span>
</p>

<p align="center" style="margin: 15px 0;">
  <a href="https://buymeacoffee.com/pylin" target="_blank">
    <img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me a Coffee" style="height: 40px; width: 150px;">
  </a>
</p>

<p align="center" style="margin: 15px 0;">
  <a href="https://www.youtube.com/channel/UCKKhdFV0q8CV5vWUDfiDfTw" target="_blank">
    <img src="https://img.shields.io/badge/SUBSCRIBE%20ON%20YOUTUBE-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="Subscribe on YouTube" style="height: 40px;">
  </a>
</p>

---

## **WiringPi Installation and LED Blink Code**

1. **Download the Installation Script:**
   ```bash
   wget https://raw.githubusercontent.com/papercodeIN/BananaPi/refs/heads/main/GPIO/WiringPi_Installation.sh
   ```

2. **Make the Script Executable:**
   ```bash
   chmod +x WiringPi_Installation.sh
   ```

3. **Run the Installation Script:**
   ```bash
   ./WiringPi_Installation.sh
   ```

4. **Verify WiringPi Installation:**
   ```bash
   gpio readall
   ```

5. **Set GPIO Pin 7 as Output:**
   ```bash
   gpio mode 7 out
   ```

6. **Turn the LED On:**
   ```bash
   gpio write 7 1
   ```

7. **Turn the LED Off:**
   ```bash
   gpio write 7 0
   ```

---

## **WiringPi-Python Installation**
1. **Download the Installation Script:**  
   ```bash
   wget https://raw.githubusercontent.com/papercodeIN/BananaPi/refs/heads/main/GPIO/WiringPi_Python_Installation.sh

   ```

2. **Make the Script Executable:**  
   ```bash
   chmod +x WiringPi_Python_Installation.sh
   ```

3. **Run the Installation Script:**  
   ```bash
   ./WiringPi_Python_Installation.sh
   ```
4. **Verify WiringPi-Python Installation using Blink Python Code:**  
   ```bash
   wget https://raw.githubusercontent.com/papercodeIN/BananaPi/refs/heads/main/GPIO/led_blink.py
   ```
   ### Change Pin Number as per your setup
   ```bash
   python3 led_blink.py
   ```   
---

## **RPI.GPIO Installation**
1. **Download the Installation Script:**  
   ```bash
   wget https://raw.githubusercontent.com/papercodeIN/BananaPi/refs/heads/main/GPIO/RPI_GPIO_Installation.sh

   ```

2. **Make the Script Executable:**  
   ```bash
   chmod +x RPI_GPIO_Installation.sh
   ```

3. **Run the Installation Script:**  
   ```bash
   ./RPI_GPIO_Installation.sh
   ```
4. **Verify WiringPi-Python Installation using Blink Python Code:**  
   ```bash
   wget https://raw.githubusercontent.com/papercodeIN/BananaPi/refs/heads/main/GPIO/led_blink_rpi_gpio.py
   ```
   ### Change Pin Number as per your setup
   ```bash
   python led_blink_rpi_gpio.py
   ```   
---

## M4 Berry 
```
root@bpi-m4berry:~# gpio readall
 +-----+-----+---------+------+---+ M4 Berry +---+------+---------+-----+-----+
 | I/O | wPi |   Name  | Mode | V | Physical | V | Mode |  Name   | wPi | I/O |
 +-----+-----+---------+------+---+----++----+---+------+---------+-----+-----+
 |     |     |    3.3V |      |   |  1 || 2  |   |      | 5V      |     |     |
 | 208 |   8 |   SDA.4 |   IN | 1 |  3 || 4  |   |      | 5V      |     |     |
 | 207 |   9 |   SCL.4 |   IN | 1 |  5 || 6  |   |      | 0V      |     |     |
 | 211 |   7 |  IO.211 | ALT7 | 0 |  7 || 8  | 0 | ALT2 | TxD1    | 15  | 198 |
 |     |     |      0V |      |   |  9 || 10 | 0 | ALT2 | RxD1    | 16  | 199 |
 | 226 |   0 |  IO.226 | ALT7 | 0 | 11 || 12 | 0 | ALT7 | IO.203  | 1   | 203 |
 | 227 |   2 |  IO.227 | ALT7 | 0 | 13 || 14 |   |      | 0V      |     |     |
 | 194 |   3 |  IO.194 | ALT7 | 0 | 15 || 16 | 0 | ALT2 | IO.200  | 4   | 200 |
 |     |     |    3.3V |      |   | 17 || 18 | 0 | ALT2 | IO.201  | 5   | 201 |
 | 231 |  12 |    MOSI | ALT4 | 0 | 19 || 20 |   |      | 0V      |     |     |
 | 232 |  13 |    MISO | ALT4 | 0 | 21 || 22 | 0 | ALT7 | IO.193  | 6   | 193 |
 | 230 |  14 |    SLCK | ALT4 | 0 | 23 || 24 | 0 | ALT4 | SS      | 10  | 229 |
 |     |     |      0V |      |   | 25 || 26 | 0 | ALT4 | IO.233  | 11  | 233 |
 | 210 |  30 |   SDA.3 | ALT7 | 0 | 27 || 28 | 0 | ALT7 | SCL.3   | 31  | 209 |
 | 195 |  21 |  IO.195 | ALT7 | 0 | 29 || 30 |   |      | 0V      |     |     |
 | 196 |  22 |  IO.196 | ALT7 | 0 | 31 || 32 | 0 | ALT7 | IO.192  | 26  | 192 |
 | 197 |  23 |  IO.197 | ALT7 | 0 | 33 || 34 |   |      | 0V      |     |     |
 | 204 |  24 |  IO.204 | ALT7 | 0 | 35 || 36 | 0 | ALT7 | IO.228  | 27  | 228 |
 | 202 |  25 |  IO.202 | ALT7 | 0 | 37 || 38 | 0 | ALT7 | IO.206  | 28  | 206 |
 |     |     |      0V |      |   | 39 || 40 | 0 | ALT7 | IO.205  | 29  | 205 |
 +-----+-----+---------+------+---+----++----+---+------+---------+-----+-----+
 | I/O | wPi |   Name  | Mode | V | Physical | V | Mode |  Name   | wPi | I/O |
 +-----+-----+---------+------+---+ M4 Berry +---+------+---------+-----+-----+
```

## M4 Zero
```
root@bpi-m4zero:~# gpio readall
 +-----+-----+---------+------+---+- M4Zero -+---+------+---------+-----+-----+
 | I/O | wPi |   Name  | Mode | V | Physical | V | Mode |  Name   | wPi | I/O |
 +-----+-----+---------+------+---+----++----+---+------+---------+-----+-----+
 |     |     |    3.3V |      |   |  1 || 2  |   |      | 5V      |     |     |
 | 262 |   8 |   SDA.0 |   IN | 1 |  3 || 4  |   |      | 5V      |     |     |
 | 261 |   9 |   SCL.0 |   IN | 1 |  5 || 6  |   |      | 0V      |     |     |
 | 268 |   7 |  IO.268 |  OUT | 0 |  7 || 8  | 0 | ALT3 | TxD1    | 15  | 269 |
 |     |     |      0V |      |   |  9 || 10 | 0 | ALT3 | RxD1    | 16  | 270 |
 | 226 |   0 |  IO.226 | ALT7 | 0 | 11 || 12 | 0 | ALT7 | IO.257  | 1   | 257 |
 | 227 |   2 |  IO.227 |  OUT | 0 | 13 || 14 |   |      | 0V      |     |     |
 | 267 |   3 |  IO.267 | ALT7 | 0 | 15 || 16 | 0 | ALT3 | IO.271  | 4   | 271 |
 |     |     |    3.3V |      |   | 17 || 18 | 0 | ALT3 | IO.272  | 5   | 272 |
 | 231 |  12 |    MOSI | ALT4 | 0 | 19 || 20 |   |      | 0V      |     |     |
 | 232 |  13 |    MISO | ALT4 | 0 | 21 || 22 | 0 | ALT7 | IO.66   | 6   | 66  |
 | 230 |  14 |    SLCK | ALT4 | 0 | 23 || 24 | 0 | ALT4 | SS      | 10  | 229 |
 |     |     |      0V |      |   | 25 || 26 | 0 | ALT4 | IO.233  | 11  | 233 |
 | 264 |  30 |   SDA.1 | ALT7 | 0 | 27 || 28 | 0 | ALT7 | SCL.1   | 31  | 263 |
 | 266 |  21 |  IO.266 | ALT7 | 0 | 29 || 30 |   |      | 0V      |     |     |
 | 265 |  22 |  IO.265 | ALT7 | 0 | 31 || 32 | 0 | ALT7 | IO.228  | 26  | 228 |
 | 234 |  23 |  IO.234 | ALT3 | 0 | 33 || 34 |   |      | 0V      |     |     |
 | 258 |  24 |  IO.258 | ALT7 | 0 | 35 || 36 | 0 | ALT7 | IO.71   | 27  | 71  |
 | 256 |  25 |  IO.256 | ALT7 | 0 | 37 || 38 | 0 | ALT7 | IO.260  | 28  | 260 |
 |     |     |      0V |      |   | 39 || 40 | 0 | ALT7 | IO.259  | 29  | 259 |
 +-----+-----+---------+------+---+----++----+---+------+---------+-----+-----+
 | I/O | wPi |   Name  | Mode | V | Physical | V | Mode |  Name   | wPi | I/O |
 +-----+-----+---------+------+---+- M4Zero -+---+------+---------+-----+-----+
```
