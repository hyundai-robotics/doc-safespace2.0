# Case 2 - Slot settings disabled (Internal Communication Not Connected)

## 1) Condition

Check the connection between the PROFIsafe board (BD671) and MainCom in the following cases:

- When the PROFIsafe board (BD671) is installed or replaced for the first time
- When the internal communication cable connected to the Hi7 MainCom is reconnected
- When the project file is initialized and the EtherCAT Master settings need to be configured again

## 2) Cause and Solution

The PROFIsafe board (BD671) must be connected to the MainCom. When the board is reinstalled or the internal communication settings are changed, follow the procedures below to check that the internal communication is working normally.

**Step 1)** Connect to the MainCom<br>
**Step 2)** Configure the EtherCAT Master

#### Summary of Checks by Cause

- W29202 EtherCAT Master I/O channel Slave connection error → Check the LAN cable connection
- Link/Act LED status error → Check the LAN cable and the board
- EtherCAT Master not configured → Refer to Step 2 below
- Slot configuration disabled → Refer to Steps 1 and 2 below
<p align="center">
<img src="../../_assets/trouble/slot_invalid.png"></img>
</p>

For more information, refer to the procedure below.

## 3) Procedure

### Step 1) Connect to the MainCom

Connect the MainCom and the PROFIsafe board (BD671) using the LAN cable marked in red, as shown in the figure below. Then, check the Link/Act and Speed LED status on each LAN port.

<p align="center">
<img src="../../_assets/trouble/lan_cable.png"></img>
</p>

**After booting the controller, check the LEDs:**
- Link/Act LED (green) - Blinking
- Speed LED (orange) - On

**After reconnecting the LAN cable, restart the controller.**

<br>
<br>

### Step 2) EtherCAT Master Settings

- Go to `[System]` → `[Control Parameters]` → `[Industrial Communication]` → `[EtherCAT Master Settings]`.

Check that the settings are configured as shown in the figure below:
- EtherCAT Master: ON
- Operation and Communication LEDs: ON
- Slave List: Check that **PROFINET I/O Interface** is selected

<p align="center">
<img src="../../_assets/trouble/ecat1.png"></img>
</p>
<p align="center">
<img src="../../_assets/trouble/ecat2.png"></img>
</p>

**After changing the settings, click the `[Apply]` button and restart the controller.**
