🔄 Use Your Own Network Traffic (Optional)
 ####- You can replace the default Dataset1.csv with your own network capture:

## Step-by-Step: Generate Your Own 📁Dataset1.csv

### ☑️ 1: - Install Wireshark (if you don’t have it):
####   - https://www.wireshark.org/download.html

### ☑️ 2: - Capture Your Traffic:
 - Open Wireshark.
 - Start capturing on your preferred interface (e.g., eth0, wlan0).
 - Let it run while you browse, ping, or generate traffic.
 - Stop the capture once you have enough data (a few hundred packets is fine).

### ☑️ 3: - Export to CSV:
 - Go to File → Export Packet Dissections → As CSV
 - Choose Packet Summary Line as the export type
 - - Save the file as: 📁 "Dataset1.csv"
 - - Place it in the same folder as the Java program (TrafficCaptureAnalysis/).

### ☑️ 4: - Run the Program Again:
 - javac IP_enumerate.java
 - java IP_enumerate

## ⚠️ Make sure the exported CSV contains the fields Source, Destination, and Protocol. These are case-insensitive but required for analysis.
