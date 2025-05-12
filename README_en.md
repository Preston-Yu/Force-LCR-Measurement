# LabVIEW Program for Pressure and Resistance Measurement

This guide explains how to use the `Lab1.0.vi` LabVIEW program to measure resistance and pressure using an LCR meter and a force measurement device.

---

## Chapter 1: Preparation

### Step 1: Power on all measurement devices
Ensure that both the LCR meter and the force measurement device are powered on and properly connected to the PC via USB or serial interface.



---

### Step 2: Launch NI MAX
Open **NI Measurement & Automation Explorer (NI MAX)** on your PC.

![NI MAX](./img/ni_max.jpg)

---

### Step 3: Click “Devices and Interfaces” and wait for detection
In NI MAX, click on the left-side menu **Devices and Interfaces**. Wait for all connected hardware to be detected.

![NI MAX Devices](./img/nimax_devices.jpg)

---

### Step 4: Confirm connections and note VISA names or COM ports
Ensure both the LCR meter and force measurement device are listed. Note their respective VISA resource names (e.g., `USB0::0xXXXX::...`) or COM port numbers (e.g., `COM3`).

---

## Chapter 2: Measurement

### Step 1: Open `Lab1.0.vi`
Launch LabVIEW and open the file named `Lab1.0.vi`.

---

### Step 2: If prompted, click “Run”
If LabVIEW shows a warning or dialog, click the **Run** button to start the VI.

![LabVIEW Run](./img/labview_run.jpg)

---

### Step 3: Main interface
The main interface contains:
- Device selection dropdowns
- Parameter settings (frequency, sample count, etc.)
- Real-time data plot
- Log window

![Main UI](./img/main_ui.jpg)

---

### Step 4: Select the correct VISA names or COM ports
From the dropdown lists, select the appropriate VISA resource or serial port for the LCR meter and the force measurement device.

---

### Step 5: Set measurement parameters (cannot be changed after starting)
Choose measurement settings such as frequency, integration time, and number of data points.  
⚠️ **These settings are locked once measurement begins.**

---

### Step 6: Click “START” to begin and select data save path
Click the **START** button. You will be prompted to choose a location to save the CSV output file.

---

### Step 7: Click “STOP” to end the measurement
⚠️ **Important:** Always click the **STOP** button to end the measurement before closing the program.  
Failing to do so may cause the devices to hang or become unresponsive.

---

## Chapter 3: Notes

- Confirm all devices are properly connected before each session.
- Avoid using low sampling rates unless necessary, as this may cause data lag.
- If the devices do not respond, try restarting LabVIEW or power-cycling the hardware.
- This program is tested with LCR meters and force sensors via VISA/Serial protocols. Custom drivers may be needed for other brands.

---

## License

This LabVIEW program is provided for research and academic use. For commercial licensing, please contact the author.

---

